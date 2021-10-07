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
      <h1 class="title">The Team</h1>
      <div class="team">
        <TeamCard />
        <TeamCard />
        <TeamCard />
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
