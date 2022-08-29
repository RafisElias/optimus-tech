<script lang="ts">
  const metrics = [
    {
      title: "Projetos concluídos",
      value: "400+",
      description: "Nós ajudamos a construir mais de 400 projetos incríveis.",
    },
    {
      title: "Colaboradores",
      value: "100+",
      description:
        "Temos mais de 100 colaboradores no nosso time que se preocupam com nossos clientes.",
    },
    {
      title: "Downloads",
      value: "20K",
      description:
        "Nossos projetos que estão disponíveis em lojas já foram baixados mais de 20.000 vezes.",
    },
    {
      title: "Reviews 5 estrelas",
      value: "500+",
      description:
        "Estamos orgulhosos de contar com mais de 500 reviews 5 estrelas em nossos produtos.",
    },
  ];
</script>

<section class="container">
  {#each metrics as metric}
    <div class="container-item">
      <h2>{metric.value}</h2>
      <span class="title">{metric.title}</span>
      <p class="description">{metric.description}</p>
    </div>
  {/each}
</section>

<style>
  .container {
    display: flex;
    justify-content: center;
    gap: 2rem;
    padding-inline: 7rem;
    padding-bottom: 6rem;
    flex-wrap: wrap;
  }

  .container-item {
    display: flex;
    flex: 1;
    flex-direction: column;
    gap: 12px;
  }

  .container-item h2 {
    color: var(--cls-red-500);
    letter-spacing: -0.02em;
    line-height: var(--lh-72);
    font-weight: var(--fw-semibold);
    font-size: var(--fs-900);
  }

  .title {
    font-size: var(--fs-500);
    line-height: var(--lh-28);
    font-weight: var(--fw-medium);
    color: var(--cls-gray-900);
  }
</style>
