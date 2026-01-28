 .............. 

 
/* Fonts */
:root {
  --default-font: "Roboto",  system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
  --heading-font: "Raleway",  sans-serif;
  --nav-font: "Poppins",  sans-serif;
}

/* Global Colors - The following color variables are used throughout the website. Updating them here will change the color scheme of the entire website */
:root { 
  --background-color: #ffffff; /* Background color for the entire website, including individual sections */
  --default-color: #444444; /* Default color used for the majority of the text content across the entire website */
  --heading-color: #555555; /* Color for headings, subheadings and title throughout the website */
  --accent-color: #3fbbc0; /* Accent color that represents your brand on the website. It's used for buttons, links, and other elements that need to stand out */
  --surface-color: #ffffff; /* The surface color is used as a background of boxed elements within sections, such as cards, icon boxes, or other elements that require a visual separation from the global background. */
  --contrast-color: #ffffff; /* Contrast color for text, ensuring readability against backgrounds of accent, heading, or default colors. */
}

/* Nav Menu Colors - The following color variables are used specifically for the navigation menu. They are separate from the global colors to allow for more customization options */
:root {
  --nav-color: #444444;  /* The default color of the main navmenu links */
  --nav-hover-color: #3fbbc0; /* Applied to main navmenu links when they are hovered over or active */
  --nav-mobile-background-color: #ffffff; /* Used as the background color for mobile navigation menu */
  --nav-dropdown-background-color: #ffffff; /* Used as the background color for dropdown items that appear when hovering over primary navigation items */
  --nav-dropdown-color: #444444; /* Used for navigation links of the dropdown items in the navigation menu. */
  --nav-dropdown-hover-color: #3fbbc0; /* Similar to --nav-hover-color, this color is applied to dropdown navigation links when they are hovered over. */
}

/* Color Presets - These classes override global colors when applied to any section or element, providing reuse of the sam color scheme. */

.light-background {
  --background-color: #f7fcfc;
  --surface-color: #ffffff;
}

.dark-background {
  --background-color: #060606;
  --default-color: #ffffff;
  --heading-color: #ffffff;
  --surface-color: #252525;
  --contrast-color: #ffffff;
}

.accent-background {
  --background-color: #3fbbc0;
  --default-color: #ffffff;
  --heading-color: #ffffff;
  --surface-color: #65c9cd;
}

/* Smooth scroll */
:root {
  scroll-behavior: smooth;
}


=================

 <!-- Appointment Section -->
<section id="appointment" class="appointment section light-background">

  <div class="container section-title" data-aos="fade-up">
    <h2>Prendre rendez-vous</h2>
    <p>Réservez votre séance avec Sofia El Mansouri à Casablanca pour un accompagnement personnalisé et naturel.</p>
  </div>

  <div class="container" data-aos="fade-up" data-aos-delay="100">

    <form action="forms/appointment.php" method="post" role="form" class="php-email-form">
      <div class="row">
        <div class="col-md-4 form-group">
          <input type="text" name="name" class="form-control" id="name" placeholder="Votre nom" required="">
        </div>
        <div class="col-md-4 form-group mt-3 mt-md-0">
          <input type="email" class="form-control" name="email" id="email" placeholder="Votre email" required="">
        </div>
        <div class="col-md-4 form-group mt-3 mt-md-0">
          <input type="tel" class="form-control" name="phone" id="phone" placeholder="Votre téléphone" required="">
        </div>
      </div>

      <div class="row">
        <div class="col-md-4 form-group mt-3">
          <input type="datetime-local" name="date" class="form-control datepicker" id="date" required="">
        </div>
        <div class="col-md-4 form-group mt-3">
          <select name="department" id="department" class="form-select" required="">
            <option value="">Sélectionnez la prestation</option>
            <option value="Naturopathie">Naturopathie</option>
            <option value="Acupuncture">Acupuncture</option>
            <option value="Réflexologie">Réflexologie</option>
            <option value="Bilan OligoScan">Bilan OligoScan / So Check</option>
            <option value="Aculifting">Aculifting</option>
            <option value="Soins énergétiques">Soins énergétiques</option>
          </select>
        </div>
        <div class="col-md-4 form-group mt-3">
          <select name="doctor" id="doctor" class="form-select" required="">
            <option value="">Votre praticienne</option>
            <option value="Sofia El Mansouri">Sofia El Mansouri</option>
          </select>
        </div>
      </div>

      <div class="form-group mt-3">
        <textarea class="form-control" name="message" rows="5" placeholder="Message ou précision (optionnel)"></textarea>
      </div>
      <div class="mt-3">
        <div class="loading">Envoi en cours</div>
        <div class="error-message"></div>
        <div class="sent-message">Votre demande de rendez-vous a bien été envoyée. Je vous recontacte rapidement.</div>
        <div class="text-center"><button type="submit">Envoyer la demande</button></div>
      </div>
    </form>

  </div>

</section><!-- /Appointment Section -->
