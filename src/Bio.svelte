<script>
  import { fade } from 'svelte/transition'
</script>

<div class='bio-container'>
  <div class='bio' in:fade={{delay: 300, duration: 500}} out:fade>
    <p>El proyecto AgileTalk comenzó en 2020 como una competencia entre dos equipos de aproximadamente 30 desarrolladores cada uno. Todos alumnos de la carrera de Ingeniaria en Sistemas de la Universidad Nacional del Centro de la Provincia de Buenos Aires, siendo parte de la materia Diseño de Software. La competencia concistió en presentar un ambiente virtual 3D didactico que permitiera a otros alumnos interiorizarse en distintos procesos de desarrollo ágil (idealmente pudiendo definirlos dentro del ambiente). Esto manteniendo una organización y siguiendo un proceso. La competencia nos dejó con dos acercamientos similares, dado que los requerimientos se fueron dando a lo largo de la cursada a ambos equipos por igual, durante las clases.</p>
    <p>A comienzos del 2021, dentro del marco de la materia Ingenieria de Sofware, la premisa fue encarar un nuevo desarrollo, pudiendo tomar como base los desarrollados en el 2020, siguiendo los elementos escenciales de SAFe (<a href='https://www.scaledagileframework.com/' target="_blank" rel="noopener noreferrer" style="color: orangered;">Scaled Agile Framework</a>) unificando ambos grupos en una pequeña empresa de 37 empleados. </p>
  </div>
</div>

<style>

  .bio {
    box-sizing: border-box;
    width: 100%;
    display: flex;
    flex: 1;
    flex-direction: column;
    justify-content: center;
    padding: 0 100px;
  }

  .bio-container  {
    position: absolute;
    height: 100%;
    display: flex;
  }

  @media only screen and (max-width: 1000px) {

    .bio {
      display: block;
      padding: 15px;
    }

    .bio-container {
      display: block;
    }
  }
</style>
