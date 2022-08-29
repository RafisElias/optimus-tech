<script lang="ts">
  import equipe from "assets/images/equipe.avif";

  const openRecruitment = [
    {
      recruitment: "Design",
      options: [
        {
          name: "Product Designer",
          type: "Full-time",
          wage: 7000,
        },
        {
          name: "UX Designer",
          type: "Full-time",
          wage: 6000,
        },
      ],
    },
    {
      recruitment: "Desenvolvimento de Software",
      options: [
        {
          name: "Desenvolvedor(a) iOS",
          type: "Full-time",
          wage: 8000,
        },
        {
          name: "Desenvolvedor(a) Front-end",
          type: "Full-time",
          wage: 7000,
        },
        {
          name: "Desenvolvedor(a) Back-end",
          type: "Full-time",
          wage: 8000,
        },
      ],
    },
  ];
</script>

<main>
  <section class="talents-container">
    <div>
      <h2 class="container-title">Estamos procurando por talentos</h2>
      <span class="chip">Vagas abertas!</span>
      <p class="about-us">
        Somos uma equipe 100% remota com pessoas do Brasil inteiro.
      </p>
    </div>
    <img src={equipe} alt="" class="equipe" />
  </section>

  <section class="jobs-container">
    {#each openRecruitment as item}
      <div class="job-item">
        <h3 class="recruitment-title">{item.recruitment}</h3>
        <ul class="recruitment-options">
          {#each item.options as option}
            <li>
              <span class="recruitment-name">{option.name}</span>
              <div>
                <span class="recruitment-type">{option.type}</span>
                <span class="recruitment-wage"
                  >Faixa salarial: {option.wage.toLocaleString("pt-br", {
                    style: "currency",
                    currency: "BRL",
                  })}</span
                >
              </div>
            </li>
          {/each}
        </ul>
      </div>
    {/each}
  </section>
</main>

<style>
  main {
    padding: 6rem 5rem;
  }
  .talents-container {
    padding-inline: 3rem;
  }

  .talents-container > div {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1rem;
  }

  .container-title {
    font-size: var(--fs-600);
    line-height: var(--lh-44);
    font-weight: var(--fw-semibold);
    text-align: center;
    color: var(--cls-gray-900);
    letter-spacing: -0.02em;
  }

  .about-us {
    text-align: center;
    font-size: var(--fs-550);
    line-height: var(--lh-30);
    margin-top: 0.25rem;
  }

  .equipe {
    margin-top: 4rem;
    aspect-ratio: 1216 / 400;
  }

  .jobs-container {
    margin-top: 4rem;
    display: flex;
    flex-direction: column;
    gap: 4rem;
    max-width: 768px;
    margin-inline: auto;
  }

  .job-item {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  .recruitment-title {
    font-weight: var(--fw-medium);
    color: var(--cls-gray-900);
    font-size: var(--fs-550);
    line-height: var(--lh-30);
  }

  .recruitment-options li {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    border: 1px solid #eaecf0;
    border-radius: 1rem;
    padding: 1.5rem 1.5rem 1.75rem;
  }

  .recruitment-options > li + li {
    /* background-color: red; */
    margin-top: 1.5rem;
  }

  .recruitment-name {
    font-weight: var(--fw-medium);
    color: var(--cls-gray-900);
    font-size: var(--fs-500);
    line-height: var(--lh-28);
  }

  .recruitment-type,
  .recruitment-wage {
    font-weight: var(--fw-medium);
    color: var(--cls-gray-500);
    font-size: var(--fs-400);
    line-height: var(--lh-24);
  }

  .recruitment-type {
    margin-right: 1.5rem;
  }
</style>
