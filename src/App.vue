<template class="template">
  <HomeView />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import HomeView from './views/HomeView.vue';


export default defineComponent({
  name: "App",
  components: { HomeView }
}
);
</script>

<style>
.form-button {
  display: flex;
  justify-content: center;
  margin-top: 1.25rem;
}

.btn-small {
  width: 9.25rem;
  height: 2.5rem;
  color: #fff;
  background-color: #FC7071;
  border: none;
  border-radius: 6px;
  font-weight: 600;
  line-height: 1.5em;
  margin: 10px;
}

.btn-large {
  width: 11.25rem;
  height: 2.5rem;
  font-family: 'Poppins', sans-serif;
  font-weight: 600;
  font-size: 1rem;
  line-height: 1.5em;
  color: #fff;
  background-color: #FC7071;
  border: none;
  border-radius: 6px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  filter: drop-shadow(2px 2px 4px rgba(0, 0, 0, 0.25));
}

.text__span {
  color: #3772FF;
  line-height: 1.25em;
  font-family: 'Poppins';
  text-align: center;
  top: 20%;
  width: 16rem;
  position: absolute;
  left: 17%;
  display: flex;
  z-index: -1;
}

@media (min-width: 768px) {

  .btn-small {
    width: 10.875rem;
    height: 2.5rem;
  }

  .btn-large {
    width: 22.625rem;
    height: 3rem;
    font-size: 1.125em;
  }
}


/**A PARTIR DAQUI O ESTILO É COPIADO DO SCREENREGISTER, LEMBRAR DE REMOVER */


html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}

body {
  line-height: 1;
}

ol,
ul {
  list-style: none;
}

blockquote,
q {
  quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
  content: '';
  content: none;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

main {
  margin: 0;
}
</style>
