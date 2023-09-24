<template>
  <section id="hero">
    <div class="img-art">
     
      <article>
        <div class="name">
          <h3>HEY, I AM</h3>
          <h1>Abubakar Abdullahi</h1>
          <h2>I'm a Data Analyst</h2>
          
        </div>
        <p>Hi there! I’m a Data Analyst with fervor for exploring and  <br>transforming raw data into actionable and valuable insights,<br> I’m adept at utilizing tools such as Python, SQL,<br> Power Bi and Microsoft tools Read more</p>
        <div class="cta">
          <a href="#"><button>Get in touch</button></a>
          <a href="#"><button>Projects</button></a>
        </div>
      </article>
      <div class="img">
        <img src="../static/img.jpg" alt="banner image" style="height: 400px;">
      </div>
    </div>
  </section>
</template>
<style>
#hero{
  margin-top: 1em;
}
#hero .img-art{
  display: flex;
  width: 100%;
  align-self: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 50px;
}
#hero .img-art article .name h1,h2, h3{
 margin: 0;
 padding: 5px;
}
#hero .img-art img{
  border-radius: 200px;
}
</style>
