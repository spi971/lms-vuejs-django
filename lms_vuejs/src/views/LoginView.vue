<template>
    <div>
      <section class="hero is-primary is-small">
        <div class="hero-body has-text-centered">
          <h1 class="title">
            Login
          </h1>
        </div>
      </section>
      <section class="section">
      <div class="container">
        <div class="columns">
          <div class="column is-4 is-offset-4">
            <form>
              <div class="field">
                <label for="email">Email</label>
                <div class="control">
                  <input type="email" name="email" id="email" class="input">
                </div>
              </div>

              <div class="field">
                <label for="password">Password</label>
                <div class="control">
                  <input type="password" name="password" id="password" class="input">
                </div>
              </div>

              <div class="field">
                <div class="control has-text-centered">
                  <button class="button is-primary">Log in</button>
                </div>
              </div>
            </form>
            <hr>
              Or <router-link to="/signup">click here</router-link> to sign up.
          </div>
        </div>
      </div>
    </section>
    </div>
  </template>