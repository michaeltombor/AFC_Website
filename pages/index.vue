<template>
  <div>
    <section class="">
      <NavBar /> 
    
      <div class="concept">
        <p class="concept_text">
          A Collection of 10.000 NFTs that let you play football with play2earn mechanics.
        </p>
        <div class="concept_animation"></div>
      </div>
      <div class="mint">
        <a href="something" class="button"
          >Coming Soon <i class="fas fa-football-ball"></i
        ></a>
      </div>
    </section>
    <section>
      <svg
        class="divider-svg"
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path d="M1200 0L0 0 892.25 114.72 1200 0z" class="shape-fill"></path>
      </svg>
      <h1 class="title">About the Ape Football Club</h1>

      <div class="about">
        <img class="about_image" src="~/assets/images/afc1.png" />
        <p class="about_text">
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
          tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At
          vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
          no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit
          amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
          labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam
          et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata
          sanctus est Lorem ipsum dolor sit amet.
        </p>
      </div>
    </section>
    <section>
      <svg
        class="divider-svg"
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path d="M1200 0L0 0 892.25 114.72 1200 0z" class="shape-fill"></path>
      </svg>
      <h1 class="title">The Roadmap</h1>
      <div class="roadmap">
        <RoadmapGoal
          :percentage="10"
          :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
        />
        <RoadmapGoal
          :percentage="20"
          :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
        />
        <RoadmapGoal
          :percentage="40"
          :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
        />
        <RoadmapGoal
          :percentage="60"
          :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
        />
        <RoadmapGoal
          :percentage="80"
          :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
        />
        <RoadmapGoal
          :percentage="100"
          :goal="'Doggo ipsum long bois lotsa pats blep. What a nice floof ruff super chub very good spot, the neighborhood pupper lotsa pats. Borkdrive shibe shoober what a nice floof, borking doggo.'"
        />
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
import RoadmapGoal from "@/components/RoadmapGoal.vue";
import Divider from "@/components/Divider.vue";
import TeamCard from "@/components/TeamCard.vue";

export default {
  components: {
    NavBar,
    RoadmapGoal,
    TeamCard,
    Divider,
  },
};
</script>
