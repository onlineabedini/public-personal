<template>
  <div>
    <div class="background p-5">
      <div class="container-fluid">
        <!-- main content -->
        <div class="row m-0">
          <!-- col2 -->
          <div class="col-2 p-0 m-0">
            <div class="p-0">
              <img class="img-fluid rounded w-100 h-100"
                src="data:image/jpeg;base64,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"
                alt="onlineabedini" />
            </div>
          </div>
          <!-- col2 -->
          <!-- col6 -->
          <div class="col-6 px-0">
            <div class="rounded px-5">
              <h1>{{ full_name }}</h1>
              <h5>{{ bio }}</h5>
              <hr />
              <h5>درباره من</h5>
              <small>
                {{ about }}
              </small>
            </div>
          </div>
          <!--/ col6 -->
          <!-- col4 -->
          <div class="col-4 p-0 m-0">
            <div class="form_div w-100 rounded-3 p-5">
              <form>
                <div class="login_title">عضویت در خبرنامه / اخبار</div>
                <div class="form-text pb-3">
                  در خبرنامه عضو شوید و از آخرین اخبار، تخفیف ها و خدمات من با خبر باشید
                </div>
                <div class="form-group mb-2">
                  <input class="form-control" type="email" placeholder="پست الکترونیکی" v-model="register_email" />
                </div>
                <div class="btn btn-outline-light px-4 py-2" @click="register_Newsletters()">ثبت</div>
                <div>
                  <small>
                    {{ register_alert }}
                  </small>
                </div>
              </form>
            </div>
          </div>
          <!--/ col4 -->
        </div>
        <!--/ main content -->
        <!-- copy right -->
        <div class="copy-right mt-5 py-3">
          <h6>
            طراحی شده توسط آنلاین عابدینی / حق کپی رایت محفوظ است
          </h6>
        </div>
        <!--/ copy right -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      full_name: "برنامه نویس نمونه",
      bio: "برنامه نویس فول استک حرفه ای",
      about: `
      لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد، کتابهای زیادی در شصت و سه درصد گذشته حال و آینده، شناخت فراوان جامعه و متخصصان را می طلبد، تا با نرم افزارها شناخت بیشتری را برای طراحان رایانه ای علی الخصوص طراحان خلاقی، و فرهنگ پیشرو در زبان فارسی ایجاد کرد، در این صورت می توان امید داشت که تمام و دشواری موجود در ارائه راهکارها، و شرایط سخت تایپ به پایان رسد و زمان مورد نیاز شامل حروفچینی دستاوردهای اصلی، و جوابگوی سوالات پیوسته اهل دنیای موجود طراحی اساسا مورد استفاده قرار گیرد.
        `,

      // form variable
      register_alert: "",
      register_email: "",
    }
  },
  methods: {
    register_Newsletters() {
      if (this.register_email) {
        this.register_alert = "شما با موفقیت عضو شدید";
      } else {
        this.register_alert = "لطفا ایمیل خود را وارد کنید";
      }
    }
  }
}
</script>
<style scoped>
.background {
  background-color: rgb(39, 39, 39);
  color: white;
}

hr {
  background-color: rgba(255, 255, 255, 0.336);
}

/* login form */
.login_title {
  font-weight: bold;
  margin-bottom: 10px;
  font-size: 18px;
}

.form-text {
  color: white;
}

input {
  color: black;
  font-weight: bold;
  letter-spacing: 2px;
}

/* copy right */
.copy-right {
  border-top: 1px solid rgba(255, 255, 255, 0.053);
}

.form_div {
  box-shadow: 0px 0px 5px black;
}
</style>
