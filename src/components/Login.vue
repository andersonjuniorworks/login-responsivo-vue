<template>
  <main>
    <section class="container">
      <div class="panel">
        <div class="panel--left">
          <img
            src="https://i.ibb.co/SV2v1G8/background.png"
            alt="imagem de fundo"
          />
        </div>
        <div class="panel--right">
          <div class="panel__header">
            <h2>Login</h2>
            <p>Forneça seus dados abaixo e aprecie uma experiência incrível</p>
          </div>
          <form class="form">
            <div class="form__group">
              <label for="email">Email</label>
              <input
                type="email"
                class="form__control"
                placeholder="Digite seu email"
                id="email"
              />
            </div>
            <div class="form__group">
              <label for="password">Senha</label>
              <input
                type="password"
                class="form__control"
                placeholder="Digite sua senha"
                id="password"
              />
            </div>
            <div class="form__action">
              <button class="button button--primary button--rounded">
                Entrar
              </button>
              <a href="#">Esqueci minha senha</a>
            </div>
          </form>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'Login',
};
</script>

<style scoped>
.container {
  position: absolute;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.panel {
  position: relative;
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.panel--left {
  width: 50%;
  height: 100vh;
}

.panel--left img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: bottom;
  transition: ease-in-out 0.3s;
}

.panel--right {
  width: 50%;
  height: 100vh;
  padding: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: ease-in-out 0.3s;
}

.panel__header {
  width: 100%;
  max-width: 350px;
  line-height: 20px;
}

.panel__header h2 {
  font-size: 35px;
  margin: 0;
}

.form {
  width: 100%;
  max-width: 350px;
  padding: 20px;
}

.form__group {
  margin: 0 0 10px 0;
  display: flex;
  flex-direction: column;
  row-gap: 5px;
}

.form__group label {
  font-weight: 500;
  font-size: 14px;
}

.form__control {
  width: calc(100% - 30px);
  height: 40px;
  padding: 0 15px;
  border-radius: 5px;
  border: 1px solid rgba(233, 233, 233, 0.7);
  outline: none;
  transition: ease-in 0.2s;
}

.form__control:focus {
  box-shadow: 0px 0px 15px 2px rgba(233, 233, 233, 1);
}

.form__action {
  width: 100%;
  margin: 35px 0 0 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  row-gap: 15px;
}

.form__action a {
  font-weight: 400;
  font-size: 14px;
  text-decoration: none;
  color: #000;
}

.form__action a:hover {
  text-decoration: underline;
}

.button {
  width: 100%;
  height: 40px;
  outline: none;
  border: none;
  font-size: 14px;
  font-weight: 500;
  transition: ease-in-out 0.2s;
}

.button--primary {
  background: #4c4f56;
  color: #fff;
}

.button--rounded {
  border-radius: 30px;
}

.button:hover {
  cursor: pointer;
  background: #272b34;
}

@media screen and (max-width: 768px) {
  .panel--left {
    display: none;
  }
  .panel--right {
    width: inherit;
  }
}
</style>
