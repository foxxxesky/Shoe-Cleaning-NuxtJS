<template>
  <section id="grid-right">
    <div class="row justify-content-center p-5">
      <div class="col-9 pt-5">
        <h4 id="text-masuk" class="pb-4">Masuk</h4>
        <!-- Form Masuk -->
        <form action="#" method="POST">
          <div class="form">
            <!-- Email -->
            <div class="mb-4">
              <label for="Email" id="form-text" class="form-label"
                >Alamat Email</label
              >
              <input type="email" class="form-control" name="email" autofocus />
            </div>

            <!-- Password -->
            <div class="mb-4">
              <label for="Password" id="form-text" class="form-label"
                >Password</label
              >
              <input type="password" class="form-control" name="password" />
            </div>

            <!-- Button -->
            <div class="mb-4">
              <button
                id="login-button"
                type="submit"
                name="Masuk"
                class="btn btn-primary"
              >
                Masuk
              </button>
            </div>
          </div>
        </form>
        <div class="mb-4">
          <p id="link-text-register" class="text-center">
            Belum punya akun?
            <nuxt-link id="link-page" to="/user/register">Daftar</nuxt-link>
          </p>
        </div>
      </div>
    </div>
  </section>
  <!-- Right Content -->
</template>

<script>
export default {
  layout: "auth",
  head() {
    return {
      title: "Login",
      head() {
        return {
          link: [{ rel: "icon", href: "images/char.png" }],
        };
      },
    };
  },
};
</script>

<style>
#text-masuk {
  font-size: 36px;
  font-weight: var(--bold);
  color: var(--primary-text);
}

#form-text {
  font-size: 18px;
  color: var(--primary-text);
}

#login-button {
  color: var(--white);
  width: 100%;
  font-size: 20px;
  font-weight: var(--semi-bold);
}

#link-text-register {
  font-size: 14px;
  font-weight: var(--medium);
  color: var(--primary-text);
}
</style>
