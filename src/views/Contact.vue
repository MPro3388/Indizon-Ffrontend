<template>
  <div class="home">
    <img alt="Blue Shield logo" src="../assets/BlueShield.png">
    <HelloWorld msg="Contact Formular"/>

    <form id="contact">
      <label id="h2" form="contact">Kontaktformular</label>
      <fieldset>
        <legend>Name</legend>

        <label for="vorname">
          Vorname: <input name="vorname" id="vorname" placeholder="Max">
        </label>

        <label for="nachname">
          Zuname: <input name="nachname" id="nachname" placeholder="Mustermann">
        </label>

      </fieldset>

      <fieldset>
        <legend>Geburtsdatum</legend>

        <label for="birth">
          Vorname: <input name="birth" id="birth" placeholder="TT.MM.JJJJ">
        </label>

      </fieldset>

      <fieldset>
        <legend>Geschlecht</legend>

        <label for="männl">
          <input type="radio" name="geschlecht" id="männl" value="männl">
          männlich
        </label>

        <label for="weibl">
          <input type="radio" name="geschlecht" id="weibl" value="weibl">
          weiblich
        </label>

      </fieldset>

      <h1>Anliegen</h1>
      <p>Schreiben Sie ihr Anliegen</p>
      <textarea cols="50" rows="10"></textarea>

      <button type="reset">Eingaben zurücksetzen</button>
      <button type="submit">Eingaben absenden</button>
    </form>

  </div>
</template>
<style>
#contact{
  position: relative;
  left: 35%;
  width: 500px;
  height: 500px;
}
</style>
