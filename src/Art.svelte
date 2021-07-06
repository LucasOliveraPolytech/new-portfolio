<script>
  import Works from './components/Works.svelte'

  const organization = [
    {
      title: "Nivel de Programa",
      description: "<p>El nivel de programa se compuso por Lucas Olivera (Product Manager), Magalí Boulanger (Release Train Engineer) y Joshua Corino (System Architect)<p>",
      outLink: "",
      media: "images/a_dark.png"
    },
    {
      title: "Croissant",
      description: "<p>El equipo Croissant compuesto por Martin Lorenzo (Product Owner), Federico Gregorio (Scrum Master), Ramiro Orella, Santiago Ithurralde, Eliel Viviant y Leonel Benavidez.</p>",
      outLink: "",
      media: "images/a_dark.png"
    },
    {
      title: "Mignon",
      description: "<p>El equipo Mignon compuesto por Erick Anderson (Product Owner), Sofía Barceló (Scrum Master), Benjamin Figeired, Lautaro Osinaga, Mainque Menjoulou y Juan Pablo Correa.</p>",
      outLink: "https://vimeo.com/401470006",
      media: "images/sestina-score.jpg"
    },
    {
      title: "Herrajería",
      description: "<p>El equipo \"Herrajeria 'La florida decoraciones'\" compuesto por Exequiel Herrera (Product Owner), Gabriel Gonzalez (Scrum Master), Thomas Ojeda, Carlos Aranda y Juan Martín Tripodi.<p>",
      media: "images/or-what-score.jpg",
      outLink: "https://vimeo.com/349680153"
    },
    {
      title: "Logistica",
      description: "<p>El equipo \"Logística 'El luchador'\" compuesto por Matias Guerrero (Product Owner), Bruno Guidi (Scrum Master), Belen Velazquez, Dana Alvarez Y Martinez y Matias Morandeira.<p>",
      media: "images/or-what-score.jpg",
      outLink: "https://vimeo.com/349680153"
    },
    {
      title: "Radio",
      description: "<p>El equipo \"Radio Oteando desde el Carajo\" compuesto por Ezequiel Carbajo (Product Owner), Martin Visca (Scrum Master), Ariel Betino y Elias Gatica.<p>",
      media: "images/99-score.jpg",
      outLink: "https://vimeo.com/349680536",
    },
    {
      title: "Sarasa",
      description: "<p>El equipo \"Sarasa Arquitectos\" compuesto por Galo Pianciola (Product Owner), Joaquin Saralegui (Product Manager), Palmira Benavente (Release Train Engineer), Nicolas Errea y Mauro Andres<p>",
      media: "images/99-score.jpg",
      outLink: "https://vimeo.com/349680536",
    },
    {
      title: "Persistencia",
      description: "<p>El equipo de persistencia compuesto por Joaquin Mastropierro y Guido Chiara<p>",
      media: "images/99-score.jpg",
      outLink: "https://vimeo.com/349680536",
    },
  ]

  let uid = 1
  
  organization.forEach((org) => {
    org.uid = uid++
  })
</script>

<Works works={organization} />
