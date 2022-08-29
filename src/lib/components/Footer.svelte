<script lang="ts">
  const postForm = () => {
    console.log("faadasds");
  };
</script>

<footer>
  <form on:submit|preventDefault={postForm}>
    <fieldset>
      <legend>
        <div>
          <h2>Acompanhe as nossas oportunidades</h2>
          <p>Seja o primeiro a saber quando novas vagas serão abertas!</p>
        </div>
      </legend>
      <div class="field">
        <label for="email" style="display: none;" />
        <input type="email" name="email" id="email" placeholder="Seu e-mail" />
        <button class="btn" type="submit">Cadastrar</button>
      </div>
    </fieldset>
  </form>
  <span class="copyright"
    >© 2022 OptimusTech. Todos os direitos reservados.</span
  >
</footer>

<style>
  footer {
    padding-block: 6rem;
    background-color: var(--cls-gray-50);
    box-shadow: 0 0 0 100vw var(--cls-gray-50);
    clip-path: inset(0 -100vw);
  }

  fieldset {
    border: none;
  }

  legend {
    margin-inline: auto;
  }

  legend h2 {
    font-size: 2.75rem;
    font-weight: var(--fw-semibold);
    line-height: var(--lh-30);
    text-align: center;
    letter-spacing: -0.02em;
    color: var(--cls-gray-900);
    margin-bottom: 1.25rem;
  }

  legend p {
    font-size: var(--fs-550);
    line-height: var(--lh-30);
    text-align: center;
  }

  .field {
    margin-inline: auto;
    margin-top: 2.5rem;
    margin-bottom: 2rem;
    width: fit-content;
    display: flex;
    gap: 0.5rem;
  }

  .field input {
    width: 22.5rem;
    height: 3rem;
    padding: 0.75rem 0.875rem 0.75rem 1rem;
    background-color: transparent;
    color: var(--cls-gray-500);
    border-radius: 0.5rem;
    border: 1px solid #d0d5dd;
    box-shadow: 0px 1px 2px rgba(16, 24, 40, 0.05);
  }

  input::placeholder {
    color: var(--cls-gray-500);
  }

  .copyright {
    display: block;
    text-align: center;
    color: var(--cls-gray-400);
    font-size: var(--fs-400);
  }
</style>
