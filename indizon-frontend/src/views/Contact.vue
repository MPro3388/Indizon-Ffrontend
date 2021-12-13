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
    </form>

  </div>
</template>
