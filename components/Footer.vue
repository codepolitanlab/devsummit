<template>
  <div>
    <footer class="space--sm border-top pb-5">
      <b-container class="text-left text-center-xs">
        <b-row cols="2" cols-md="4" class="container">
          <b-col>
            <h6 class="type--uppercase mt-5 mb-2">
              Join Us!
            </h6>
            <ul class="list--hover list-group">
              <li>
                <a target="_blank" href="https://www.codepolitan.com/cara-belajar">
                  Cara Belajar
                </a>
              </li>
              <li>
                <a target="_blank" href="https://www.codepolitan.com/tnc">
                  Terms & Conditions
                </a>
              </li>
              <li>
                <a target="_blank" href="https://www.codepolitan.com/faq">
                  Frequently Asked Questions
                </a>
              </li>
              <li>
                <a target="_blank" href="https://www.codepolitan.com/privacy-policy">
                  Privacy Policy
                </a>
              </li>
            </ul>
          </b-col>
          <b-col>
            <h6 class="type--uppercase mt-5 mb-2">
              Program
            </h6>
            <ul class="list--hover list-group">
              <li><a target="_blank" href="https://devschool.id/">Developer School</a></li>
              <li><a target="_blank" href="https://kampuscoding.id/">Kampus Coding</a></li>
              <li><a target="_blank" href="https://geekmentor.id/">Online Mentoring</a></li>
            </ul>
          </b-col>
          <b-col>
            <h6 class="type--uppercase mt-5 mb-2">
              Developers
            </h6>
            <ul class="list--hover list-group">
              <li>
                <a target="_blank" href="https://www.codepolitan.com/forum">
                  Forum Discussions
                </a>
              </li>
              <li>
                <a target="_blank" href="https://www.codepolitan.com/credit-to-bug-reporter">
                  Hall of Fame
                </a>
              </li>
              <li>
                <a target="_blank" href="https://www.codepolitan.com/leaderboard">
                  Leaderboard
                </a>
              </li>
            </ul>
          </b-col>
          <b-col>
            <h6 class="type--uppercase mt-5 mb-2">
              Company
            </h6>
            <ul class="list--hover list-group">
              <li>
                <a target="_blank" href="https://www.codepolitan.com/about">
                  About Codepolitan
                </a>
              </li>
              <li>
                <a target="_blank" href="https://www.codepolitan.com/articles">
                  Blog
                </a>
              </li>
            </ul>
          </b-col>
        </b-row>
      </b-container>
    </footer>
    <footer id="bottom" class="border-top">
      <div class="container pt-3">
        <b-row>
          <b-col cols="6">
            <span class="type--fine-print">© <span class="update-year">2018</span> CodePolitan. All rights reserved</span>
          </b-col>
          <b-col cols="5" class="text-left-xs">
            <b-row class="list--hover justify-content-end">
              <b-col cols="1">
                <a target="_blank" href="https://www.facebook.com/codepolitan/"><b-icon icon="facebook" font-scale="1.5" /></a>
              </b-col>
              <b-col cols="1">
                <a target="_blank" href="https://www.instagram.com/codepolitan/"><b-icon icon="instagram" font-scale="1.5" /></a>
              </b-col>
              <b-col cols="1">
                <a target="_blank" href="https://twitter.com/codepolitan"><b-icon icon="twitter" font-scale="1.5" /></a>
              </b-col>
              <b-col cols="1">
                <a target="_blank" href="https://www.linkedin.com/company/codepolitan"><b-icon icon="linkedin" font-scale="1.5" /></a>
              </b-col>
              <b-col cols="1">
                <a target="_blank" href="https://www.youtube.com/c/codepolitan"><b-icon icon="youtube" font-scale="1.6" /></a>
              </b-col>
            </b-row>
          </b-col>
        </b-row>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
footer.space--sm {
  padding-top: 0 !important;
}
#bottom {
  padding-bottom: 10px !important;
  padding-top: 0 !important;
}
.type--uppercase {
  text-transform: uppercase;
}
.list--hover li {
  transition: 0.2s ease;
  -webkit-transition: 0.2s ease;
  -moz-transition: 0.2s ease;
}
.list--hover li:not(:hover) {
  opacity: .6;
}
.type--fine-print {
  font-size: 0.85714286em;
}
ul:not([class*='menu']) li > a:hover {
  text-decoration: none;
}
ul,
a {
  margin: 0;
  padding: 0;
}
ul,
ol {
  list-style: none;
  line-height: 1.85714286em;
}
a {
  color: black;
  font-weight: 700;
}
.social-list a {
  color: #252525;
}
footer a {
  font-weight: normal;
}
footer a.type--fine-print:not(:first-child) {
  margin-left: 1.85714286em;
}
</style>
