<template>
  <section>
    <b-container class="mt-5">
      <b-row>
        <b-col
          cols="12"
          sm="8"
          offset-sm="2"
          md="6"
          offset-md="3"
          lg="6"
          offset-lg="3"
          xl="4"
          offset-xl="4"
        >
          <div class="login-brand">
            <img src="@/assets/stisla/img/stisla-fill.svg" alt="logo" width="100" class="shadow-light rounded-circle">
          </div>
          <Card title="Login">
            <b-form>
              <b-form-group
                label="Email"
                label-for="email"
                :state="validateEmail"
                :invalid-feedback="invalidFeedback"
              >
                <b-form-input
                  id="email"
                  v-model="form.email"
                  :state="validateEmail"
                  type="email"
                />
              </b-form-group>

              <b-form-group
                label="Password"
                label-for="password"
                :state="validatePassword"
                :invalid-feedback="invalidFeedback"
              >
                <b-form-input
                  id="password"
                  v-model="form.password"
                  type="password"
                />
              </b-form-group>

              <b-form-group
                label="Remember Me"
                label-for="remember"
              >
                <b-form-checkbox
                  id="remember"
                  name="remember"
                  value="accepted"
                  unchecked-value="not_accepted"
                >
                  I accept the terms and use
                </b-form-checkbox>
              </b-form-group>

              <b-form-group>
                <div class="float-right">
                  <a href="#" class="text-small">
                    Forgot Password?
                  </a>
                </div>
              </b-form-group>

              <b-form-group>
                <b-button block size="lg" variant="primary">
                  Login
                </b-button>
              </b-form-group>
            </b-form>
          </Card>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Card from '@/components/Card.vue'
export default {
  layout: 'login',
  components: {
    Card
  },
  data () {
    return {
      form: {
        email: '',
        password: ''
      }
    }
  },
  computed: {
    validateEmail () {
      return this.form.email !== ''
    },
    validatePassword () {
      return this.form.password !== ''
    },
    invalidFeedback () {
      return 'Please fill this field.'
    }
  }
}
</script>
