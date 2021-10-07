<template>
  <div>
    <section>
      <NavBar />
      <div>
        <div class="flex flex-col">
          <img class="my-4" src="~/assets/images/field.png" />
          <p class="mx-8 text-center intro">
            A Collection of 10.000 Apes that let you play football with play2earn
            mechanics.
          </p>
        </div>
      </div>

      <div class="mint mt-8">
        <a href="something" class="button"
          >Mint Soon <i class="fas fa-football-ball"></i
        ></a>
      </div>
    </section>
    <section>
      <Divider />

      <div class="container m-auto px-8 py-12">
        <h1 class="title">The Ape Football Club</h1>
        <div class="grid md:grid-flow-col about">
          <div class="pr-8">
            <p class="about_text">
              Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy
              eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam
              voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet
              clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit
              amet. Lorem ipsum dolor si voluptua. At vero eos et accusam et justo duo
              dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est
              Lorem ipsum dolor sit amet. Lorem ipsum dolor si
            </p>
            <a class="button mt-4">Join our Discord</a>
          </div>
          <ApeSlider class="mt-8" />
        </div>
      </div>
    </section>
    <section>
      <Divider />
      <div class="container m-auto px-8 py-12">
        <h1 class="title">The Roadmap</h1>
        <div class="flex flex-col">
          <RoadmapGoal
            title="Test1"
            :percentage="10"
            :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
          />
          <RoadmapGoal
            title="Test1"
            :percentage="20"
            :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
          />
          <RoadmapGoal
            title="Test1"
            :percentage="40"
            :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
          />
          <RoadmapGoal
            title="Test1"
            :percentage="60"
            :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
          />
          <RoadmapGoal
            title="Test1"
            :percentage="80"
            :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
          />
          <RoadmapGoal
            title="Test1"
            :percentage="100"
            :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
          />
        </div>
      </div>
    </section>
    <section>
      <Divider />
      <div class="m-auto px-8 py-12">
        <h1 class="title">The Team</h1>
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-4">
          <TeamCard
            name="Omar™"
            position="Visionary"
            intro="Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. "
            image="omar.jpg"
            twitter=""
            wallet=""
          />
          <TeamCard
            name="Hln_visual"
            position="Artist"
            intro="Out of a small 600 person Texas town, Harrison (HLN_Visual) is an illustrator and story teller that dabbles in just about every creative medium. He is most known for his character designs that have gone viral on tiktok and Instagram."
            image="Hln_visual.jpg"
            twitter="https://twitter.com/hln_visual"
            wallet=""
          />
          <TeamCard
            name="Allo"
            position="Developer"
            intro="Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. "
            image="allo.jpg"
            twitter="https://twitter.com/dev_allo"
            wallet="https://opensea.io/Allo-Dev"
            class="sm:col-span-4 lg:col-span-1"
          />
        </div>
      </div>
    </section>
    <section>
      <div class="flex flex-col text-center pb-4">
        <img class="h-16 m-auto" src="~/../assets/images/logo.png" />
        <div class="flex flex-row m-auto my-4 text-white gap-2">
          <a href="https://twitter.com/ApeFootballClub"><i class="fab fa-twitter fa-2x"></i></a>
          <a href="https://discord.gg/rByA8538DQ"><i class="fab fa-discord fa-2x"></i></a>
        </div>
        <p class="text-white">© ApeFootballClub - Est. 2021</p>
      </div>
    </section>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import ApeSlider from "@/components/ApeSlider.vue";

import RoadmapGoal from "@/components/RoadmapGoal.vue";
import Divider from "@/components/Divider.vue";
import TeamCard from "@/components/TeamCard.vue";

export default {
  components: {
    NavBar,
    ApeSlider,
    RoadmapGoal,
    TeamCard,
    Divider,
  },
};
</script>
