<script>
  import Works from './components/Works.svelte'

  const features = [
    {
      title: "AgileBots",
      description: "<p>El centro de AgileTalk son los llamados \"AgileBots\". En principio son agentes con la capacidad de ser personificados por un Team Member o actuar como un representante del mismo ante determinadas situaciones (reuniones, por ejemplo). Tambien hay otros que son parte del sistema como el Process Action Bot que si bien tiene un avatar dentro del mundo no puede ser personificado.</p>",
      outLink: "https://catalyticsound.com/quarterly/8/index.html",
      media: "images/cq-8.png",
    },
    {
      title: "Lenguaje Natural",
      description: "<p>AgileTalk está diseñado para que la gran parte de las interacciones se hagan dentro del ambiente virtual utilizando el lenguaje natural.</p>",
      outLink: "https://catalyticsound.com/quarterly/8/index.html",
      media: "images/cq-8.png",
    },
    {
      title: "Definición y Control de Proceso",
      description: "<p>AgileTalk puede ser configurado para seguir un proceso de desarrollo definido previamente. Dicho seguimiento está a cargo del Process Action Bot, quien tiene la característica de reportar ante el Scrum Master distintas métricas a diariamente.</p>",
      outLink: "https://catalyticsound.com/quarterly/9/index.html",
      media: "images/cq-9.png"
    },
    {
      title: "Sugerencias Arquitectónicas",
      description: "<p> </p>",
      media: "images/catalyticsoundstream.png"
    },
    {
      title: "Simulación",
      description: "<p>Dentro de AgileTalk es posible recrear el flujo de eventos luego de haberse dado dentro del ambiente, estando inmerso en el mundo al momento de la reproducción.</p>",
      media: "images/catalyticsoundstream.png"
    },
    {
      title: "Asistente de Scrum",
      description: "<p>Como herramienta didáctica, AgileTalk permite entrenar a alguien en un nuevo proceso de desarrollo guiándolo a traves de las distintas ceremonias y artefactos.</p>",
      media: "images/catalyticsoundstream.png"
    },
    {
      title: "Personalizable",
      description: "<p>Aún en desarrollo. Manteniendo un monitoreo de las distintas acciones de un Team Member a lo largo de un proyecto sería posible inferir en su personalidad y por ende personalizar sus respuestas y acciones en base a la misma cuando esté desconectado</p>",
      media: "images/catalyticsoundstream.png"
    },
  ]

  let uid = 1
  
  features.forEach((feat) => {
    feat.uid = uid++
  })
</script>

<Works works={features} />
