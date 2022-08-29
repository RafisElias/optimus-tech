<script lang="ts">
  import avatar from "assets/images/avatar.png";
</script>

<section class="testimonial-container">
  <span class="subheading">Veja o que nossos colaboradores falam sobre nós</span
  >
  <blockquote>
    <p>
      OptimusTech se importa com a saúde dos seus colaboradores e sempre procura
      nos dar todo tipo de auxílio possível.
    </p>
  </blockquote>
  <div class="attribution">
    <img src={avatar} alt="" width="56" height="56" class="avatar" />

    <span class="name">Júlia Castro</span>
    <span class="job">Desenvolvedora Web</span>
  </div>
</section>

<style>
  .testimonial-container {
    margin-inline: 2rem;
    margin-bottom: 6rem;
    padding: 4rem;
    border-radius: 1rem;
    background-color: var(--cls-red-200);
  }

  .subheading {
    color: var(--cls-red-500);
    font-weight: var(--fw-semibold);
    font-size: var(--fs-350);
    text-align: center;
    line-height: var(--lh-20);
    display: block;
  }

  blockquote {
    font-weight: var(--fw-medium);
    font-size: var(--fs-600);
    line-height: var(--lh-44);
    text-align: center;
    letter-spacing: -0.02em;
    color: #101828;
    margin-top: 1rem;
  }

  .attribution {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 2rem;
  }

  .attribution > span + span {
    margin-top: 0.25rem;
  }

  .avatar {
    width: 3.5rem;
    aspect-ratio: 1;
    margin-bottom: 1rem;
  }

  .name {
    font-size: var(--fs-400);
    font-weight: var(--fw-medium);
    text-align: center;
    color: var(--cls-gray-900);
  }

  .job {
    font-size: var(--fs-350);
    text-align: center;
    line-height: var(--lh-20);
  }
</style>
