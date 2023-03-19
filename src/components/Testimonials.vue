<script setup></script>

<template>
  <section class="testimonial-reviews">
    <!-- DANIEL -->
    <figure class="testimonial-card card-daniel">
      <figcaption class="testimonial-author">
        <img
          class="testimonial-avatar"
          src="../assets/image-daniel.jpg"
          alt="Jonathan Walters avatar image"
        />
        <div class="testimonial-author-info">
          <p class="testimonial-author-name">Daniel Clifford</p>
          <p class="testimonial-verified">Verified Graduate</p>
        </div>
      </figcaption>
      <blockquote class="testimonial-paragraph">
        <p class="testimonial-lg">
          I received a job offer mid-course, and the subjects I learned were
          current, if not more so, in the company I joined. I honestly feel I
          got every penny’s worth.
        </p>
        <p class="testimonial-sm">
          “ I was an EMT for many years before I joined the bootcamp. I’ve been
          looking to make a transition and have heard some people who had an
          amazing experience here. I signed up for the free intro course and
          found it incredibly fun! I enrolled shortly thereafter. The next 12
          weeks was the best - and most grueling - time of my life. Since
          completing the course, I’ve successfully switched careers, working as
          a Software Engineer at a VR startup. ”
        </p>
      </blockquote>
    </figure>

    <!-- JONATHAN -->
    <figure class="testimonial-card card-jonathan">
      <figcaption class="testimonial-author">
        <img
          class="testimonial-avatar"
          src="../assets/image-jonathan.jpg"
          alt="Daniel Clifford avatar image"
        />
        <div class="testimonial-author-info">
          <p class="testimonial-author-name">Jonathan Walters</p>
          <p class="testimonial-verified">Verified Graduate</p>
        </div>
      </figcaption>
      <blockquote class="testimonial-paragraph">
        <p class="testimonial-lg">
          The team was very supportive and kept me motivated
        </p>
        <p class="testimonial-sm">
          “ I started as a total newbie with virtually no coding skills. I now
          work as a mobile engineer for a big company. This was one of the best
          investments I’ve made in myself. ”
        </p>
      </blockquote>
    </figure>

    <!-- JEANETTE -->
    <figure class="testimonial-card card-jeanette">
      <figcaption class="testimonial-author">
        <img
          class="testimonial-avatar"
          src="../assets/image-jeanette.jpg"
          alt="Jeanette Harmon avatar image"
        />
        <div class="testimonial-author-info">
          <p class="testimonial-author-name">Jeanette Harmon</p>
          <p class="testimonial-verified">Verified Graduate</p>
        </div>
      </figcaption>
      <blockquote class="testimonial-paragraph">
        <p class="testimonial-lg">
          An overall wonderful and rewarding experience
        </p>
        <p class="testimonial-sm">
          “ Thank you for the wonderful experience! I now have a job I really
          enjoy, and make a good living while doing something I love. ”
        </p>
      </blockquote>
    </figure>

    <!-- PATRICK -->
    <figure class="testimonial-card card-patrick">
      <figcaption class="testimonial-author">
        <img
          class="testimonial-avatar"
          src="../assets/image-patrick.jpg"
          alt="Patrick Abrams avatar image"
        />
        <div class="testimonial-author-info">
          <p class="testimonial-author-name">Patrick Abrams</p>
          <p class="testimonial-verified">Verified Graduate</p>
        </div>
      </figcaption>
      <blockquote class="testimonial-paragraph">
        <p class="testimonial-lg">
          Awesome teaching support from TAs who did the bootcamp themselves.
          Getting guidance from them and learning from their experiences was
          easy.
        </p>
        <p class="testimonial-sm">
          “ The staff seem genuinely concerned about my progress which I find
          really refreshing. The program gave me the confidence necessary to be
          able to go out in the world and present myself as a capable junior
          developer. The standard is above the rest. You will get the personal
          attention you need from an incredible community of smart and amazing
          people. ”
        </p>
      </blockquote>
    </figure>

    <!-- KIRA -->
    <figure class="testimonial-card card-kira">
      <figcaption class="testimonial-author">
        <img
          class="testimonial-avatar"
          src="../assets/image-kira.jpg"
          alt="Kira Whittle avatar image"
        />
        <div class="testimonial-author-info">
          <p class="testimonial-author-name">Kira Whittle</p>
          <p class="testimonial-verified">Verified Graduate</p>
        </div>
      </figcaption>
      <blockquote class="testimonial-paragraph">
        <p class="testimonial-lg">
          Such a life-changing experience. Highly recommended!
        </p>
        <p class="testimonial-sm">
          “ Before joining the bootcamp, I’ve never written a line of code. I
          needed some structure from professionals who can help me learn
          programming step by step. I was encouraged to enroll by a former
          student of theirs who can only say wonderful things about the program.
          The entire curriculum and staff did not disappoint. They were very
          hands-on and I never had to wait long for assistance. The agile team
          project, in particular, was outstanding. It took my learning to the
          next level in a way that no tutorial could ever have. In fact, I’ve
          often referred to it during interviews as an example of my developent
          experience. It certainly helped me land a job as a full-stack
          developer after receiving multiple offers. 100% recommend! ”
        </p>
      </blockquote>
    </figure>
  </section>
</template>

<style scoped>
figcaption,
blockquote {
  padding: 0.45rem;
}
.testimonial-reviews {
  display: grid;
  padding: 4.5rem 1.65rem;
  gap: 1.65rem;
  max-width: 71.125rem;
}

.testimonial-card {
  box-shadow: 3px 3px 10px hsla(217, 30%, 14%, 0.281);
  border-radius: 0.625rem;
  padding: 1.25rem;
}

.testimonial-author {
  display: flex;
  padding-bottom: 1rem;
}

.testimonial-avatar {
  border-radius: 50%;
  width: 30px;
  height: 30px;
  border: 2px solid var(--light-gray);
}

.card-patrick .testimonial-avatar {
  border: 2px solid var(--moderate-violet);
}

.testimonial-author-info {
  line-height: 1rem;
  margin-left: 1rem;
}

.testimonial-author-name {
  font-size: 0.85rem;
}

.testimonial-verified {
  font-size: 0.75rem;
  opacity: 50%;
}

.testimonial-lg {
  font-size: 1.2rem;
  line-height: 1.5rem;
  font-weight: 600;
  padding-bottom: 0.95rem;
}

.testimonial-sm {
  opacity: 70%;
  font-size: 0.85rem;
  font-weight: 500;
  line-height: 1rem;
}

.card-daniel {
  background-color: var(--moderate-violet);
  background-image: url(../assets/bg-pattern-quotation.svg);
  background-repeat: no-repeat;
  background-position: right 10% top 0%;
}

.card-jonathan {
  background-color: var(--grayish-blue);
}

.card-patrick {
  background-color: var(--blackish-blue);
}

.card-jeanette,
.card-kira {
  background-color: var(--white);
  color: var(--grayish-blue);
}

.testimonial-card:hover {
  transform: scale(1.03);
  transition: 0.2ms ease;
}

@media (width >=1024px) {
  .testimonial-reviews {
    grid-template-columns: repeat(4, 1fr);
    grid-template-areas:
      "daniel daniel jonathan kira"
      "jeanette patrick patrick kira";
  }

  .card-daniel {
    grid-area: daniel;
    background-position: right 18% top 0%;
  }
  .card-jonathan {
    grid-area: jonathan;
  }
  .card-kira {
    grid-area: kira;
  }
  .card-jeanette {
    grid-area: jeanette;
  }
  .card-patrick {
    grid-area: patrick;
  }
}
</style>
