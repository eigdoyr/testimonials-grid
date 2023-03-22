<script setup>
import testimonialData from "../assets/data.json";
</script>

<template>
  <div class="testimonial">
    <figure
      :class="`testimonial-card testimonial-card-${testimonial.author.firstName}`"
      v-for="testimonial in testimonialData"
      :key="testimonial.id"
    >
      <figcaption class="testimonial-author">
        <img
          width="29"
          height="29"
          class="testimonial-avatar"
          :src="`./image-${testimonial.author.firstName}.jpg`"
          :alt="`${testimonial.author.firstName} avatar icon`"
        />
        <div class="testimonial-author-info">
          <p class="testimonial-author-name">
            {{
              testimonial.author.firstName + " " + testimonial.author.lastName
            }}
          </p>
          <p
            v-if="`${testimonial.isVerified}` === 'true'"
            class="testimonial-verified"
          >
            Verified Graduate
          </p>
        </div>
      </figcaption>
      <div>
        <p class="testimonial-main">
          {{ testimonial.testimonialMain }}
        </p>
      </div>
      <blockquote class="testimonial-paragraph">
        <p class="testimonial-lead">
          &ldquo; {{ testimonial.testimonialLead }} &rdquo;
        </p>
      </blockquote>
    </figure>
  </div>
</template>

<style scoped>
.testimonial {
  padding: 4.5rem 1.5rem;
  display: grid;
  gap: 1.5rem;
  max-width: 1154px;
}

.testimonial-card {
  padding: 1.5rem 2rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 1rem;
  color: var(--white);
  border-radius: 0.7rem;
}

.testimonial-author {
  display: flex;
  align-items: center;
  gap: 1rem;
  text-transform: capitalize;
}

.testimonial-author-name {
  font-size: 0.75rem;
}

.testimonial-verified {
  font-size: 0.75rem;
  font-weight: 600;
  /* opacity: 0.5; */
}

.testimonial-avatar {
  border-radius: 50%;
  border: 2px solid var(--white);
}

.testimonial-main {
  font-size: 1.1rem;
  font-weight: 600;
  line-height: 1.5rem;
  letter-spacing: 0.025rem;
}

.testimonial-lead {
  font-size: 0.8rem;
  font-weight: 500;
  /* opacity: 0.7; */
  line-height: 1.5;
}

.testimonial-card-daniel {
  background-color: var(--black);
  background-image: url("../assets/bg-pattern-quotation.svg");
  background-repeat: no-repeat;
  background-position: top right 10%;
}
.testimonial-card-jonathan {
  background-color: var(--dark-gray);
}
.testimonial-card-jeanette {
  background-color: var(--light-gray);
  color: var(--black);
}
.testimonial-card-patrick {
  background-color: var(--extra-light);
  color: var(--black);
}
.testimonial-card-kira {
  background-color: var(--extra-extra-light);
  color: var(--black);
}

.testimonial-card-patrick img {
  border: 2px solid var(--primary);
}

@media (width>=64rem) {
  .testimonial {
    grid-template-columns: repeat(4, 1fr);
    grid-template-areas:
      "daniel daniel jonathan kira"
      "jeanette patrick patrick kira";
    gap: 1.92rem;
    animation: 2s 1 normal slidein;
  }

  .testimonial-lead {
    font-size: 0.8rem;
    line-height: 1.45;
  }

  .testimonial-card-daniel {
    grid-area: daniel;
    background-position: top right 18%;
  }
  .testimonial-card-jonathan {
    grid-area: jonathan;
  }
  .testimonial-card-jeanette {
    grid-area: jeanette;
  }
  .testimonial-card-patrick {
    grid-area: patrick;
  }
  .testimonial-card-kira {
    grid-area: kira;
  }

  .testimonial-main {
    font-size: 1.2rem;
  }
}

@keyframes slidein {
  from {
    margin-top: 100%;
    width: 100%;
  }

  to {
    margin-top: 0%;
    width: 100%;
  }
}
</style>
