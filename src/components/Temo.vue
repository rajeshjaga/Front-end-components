<template>
  <div class="temo">
    <input type="checkbox" name="checkbox" id="checkbox" />
    <div class="color">
      <label for="checkbox">
        <i class="far fa-sun"></i>
        <i class="far fa-moon"></i>
        <div class="pointer"></div>
      </label>
    </div>
  </div>
</template>

<script>
export default {
  name: "Temo"
};
</script>

<style >
:root{
  --white:#fcfcfc;
  --black:#1c1c1c;
  --newwhite:#1c1c1c;
  --newblack:#fcfcfc;
}
body{
  height:100vh;
  width:100%;
  margin:0;
  padding:0;
}
.color{
  height:100vh;
  width:100%;
  display:flex;
  justify-content:center;
  align-items:center;
  background:var(--white);
  transition:0.35s all cubic-bezier(.17,.67,.83,.67) 0.5s;
}
input[type=checkbox]{
  display:none;
}
label{
  position:relative;
  margin:0 auto;
  font-size:1.5em;
  color:var(--white);
  background:var(--black);
  padding:0.5em 0.5em;
  display:flex;
  justify-content:space-between;
  align-items:center;
  width:3em;
  height:auto;
  border-radius:50px;
  box-shadow:0px 12px 24px rgba(0,0,0,0.14);
  transition:0.5s ease-in all 0.2s;
}

.pointer{
  position:absolute;
  z-index:1;
  height:0.25em;
  width:0.25em;
  top:0.18em;
  left:0.2em;
  padding:0.7em;
  border-radius:50px;
  background:var(--white); 
  transition:0.3s ease-in-out all;
}
input[type=checkbox]:checked + .color label .pointer{
  transform:translateX(2em);
}

input[type=checkbox]:checked +  .color {
  --white:var(--newwhite);
  --black:var(--newblack);
}
</style>
