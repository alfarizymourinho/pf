<script setup>
import { Navbar, NavbarCollapse, NavbarLink } from 'flowbite-vue'
import { TheCard } from 'flowbite-vue'
import { Toast } from 'flowbite-vue'
import { Progress } from 'flowbite-vue'
import { Avatar } from 'flowbite-vue'
import { Timeline, TimelineItem, TimelinePoint, TimelineTime, TimelineContent, TimelineTitle } from 'flowbite-vue'

</script>
<style>
@import url(//maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css);
@import url(https://fonts.googleapis.com/css?family=Roboto:400,300);

/*Ignore me, I'm just page styling*/
html {font-family: 'Roboto', sans-serif;font-size:16px;line-height:1em;height:100%;}
body {
  background: #ffffff;
  background: -moz-linear-gradient(-45deg, #ffffff 0%, #ffffff 50%, #F2F2F2 50%, #F2F2F2 50%, #F2F2F2 100%);
  background: -webkit-gradient(linear, left top, right bottom, color-stop(0%,#ffffff), color-stop(50%,#ffffff), color-stop(50%,#F2F2F2), color-stop(50%,#F2F2F2), color-stop(100%,#F2F2F2));
  background: -webkit-linear-gradient(-45deg, #ffffff 0%,#ffffff 50%,#F2F2F2 50%,#F2F2F2 50%,#F2F2F2 100%);
  background: -o-linear-gradient(-45deg, #ffffff 0%,#ffffff 50%,#F2F2F2 50%,#F2F2F2 50%,#F2F2F2 100%);
  background: -ms-linear-gradient(-45deg, #ffffff 0%,#ffffff 50%,#F2F2F2 50%,#F2F2F2 50%,#F2F2F2 100%);
  background: linear-gradient(135deg, #ffffff 0%,#ffffff 50%,#F2F2F2 50%,#F2F2F2 50%,#F2F2F2 100%);
}

h1 {font-size:1.5em;margin-bottom:55px;}

#social-platforms {
  font-size:1rem;
  text-align:center;
  overflow:hidden;
}

/*Pen code from this point on*/
.btn {
  clear:both;
  white-space:nowrap;
  font-size:.8em;
  display:inline-block;
  border-radius:5px;
  box-shadow: 0 1px 5px 0 rgba(0, 0, 0, 0.35);
  margin:2px;
  -webkit-transition:all .5s;
  -moz-transition:all .5s;
  transition:all .5s;
  overflow:hidden
}

.btn:hover {
  box-shadow: 0 5px 15px 0 rgba(0, 0, 0, 0.45);
}

.btn:focus {
  box-shadow: 0 3px 10px 0 rgba(0, 0, 0, 0.4);
}

.btn > span,.btn-icon > i {
  float:left;
  padding:13px;
  -webkit-transition:all .5s;
  -moz-transition:all .5s;
  transition:all .5s;
  line-height:1em
}

.btn > span {
  padding:14px 18px 16px;
  white-space:nowrap;
  color:#FFF;
  background:#b8b8b8
}

.btn:focus > span {
  background:#9a9a9a
}

.btn-icon > i {
  border-radius:5px 0 0 5px;
  position:relative;
  width:13px;
  text-align:center;
  font-size:1.25em;
  color:#fff;
  background:#212121
}

.btn-icon > i:after {
  content:"";
  border:8px solid;
  border-color:transparent transparent transparent #222;
  position:absolute;
  top:13px;
  right:-15px
}

.btn-icon:hover > i,.btn-icon:focus > i {
  color:#FFF
}

.btn-icon > span {
  border-radius:0 5px 5px 0
}

/*Facebook*/
.btn-facebook:hover > i,.btn-facebook:focus > i {
  color:#3b5998
}

.btn-facebook > span {
  background:#3b5998
}

/*Twitter*/
.btn-instagram:hover > i,.btn-instagram:focus > i {
  color:#dc56d3
}

.btn-instagram > span {
  background:#dc56d3
}

/*Google*/
.btn-github:hover > i,.btn-github:focus > i {
  color:#060606
}

.btn-github > span {
  background:#060606
}

</style>
<template >
    <Navbar style="background-color: steelblue;">
      <template #logo>
        <div class="flex items-center">
            <Avatar status="online" status-position="top-left" rounded img="img/three.jpg" class="mr-2.5" />
          Al-farizy M G
        </div>
      </template>
      <template #default="{isShowMenu}">    
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Beranda</NavbarLink>
          <NavbarLink><a href="#identitas">Identitas</a></NavbarLink>
          <NavbarLink><a href="#timeline">Perjalanan Hidup</a></NavbarLink>
          <NavbarLink><a href="#about">Tentang Saya</a></NavbarLink>
          <NavbarLink><a href="#talenta">Talenta Kemampuan</a></NavbarLink>
        </NavbarCollapse>
      </template>
      <template #menu-icon>
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"></path></svg>
      </template>
    </Navbar>
   
<section class="bg-center bg-no-repeat bg-[url('/img/three.jpg')] bg-gray-700 bg-blend-multiply bg-cover my-5">
    <div class="px-4 mx-auto max-w-screen-xl text-center py-24 lg:py-56">
        <h1 class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-white md:text-5xl lg:text-6xl">Kau mengenalku, maka kau membutuhkanku.</h1>
        <p class="mb-8 text-lg font-normal text-gray-300 lg:text-xl sm:px-16 lg:px-48">Violet Evergarden is the best</p>
        <div class="flex flex-col space-y-4 sm:flex-row sm:justify-center sm:space-y-0 sm:space-x-4">
            <a href="#identitas" class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-white rounded-lg bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 dark:focus:ring-blue-900">
                Get started
            </a> 
        </div>
    </div>
</section>

<Progress progress="100" class="my-5" style="margin: 5px;"></Progress>

<div class="flex" style="margin: 20px; background-color: skyblue;" id="identitas">
    <the-card variant="image" img-src="img/three.jpg" img-alt="Desk" style="background-color: steelblue;">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">IDENTITAS</h5>
    <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
    Al-farizy Mourinho Galindra
  </Toast>
  <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
    Laki-laki.
  </Toast>
  <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
   Bandung,08-03-06
  </Toast>
  <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
 17 Tahun
  </Toast>
  <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
 Islam
  </Toast>
  <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
 Pelajar
  </Toast>
  <Toast :type="'success'" style="background-color: skyblue; color: black;" class="my-3">
 Bandung, kab Bandung, Kec Margahayu, Desa Sayati.
  </Toast>
  </the-card>

  <Timeline id="timeline">
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time style="color:darkcyan;">
          Maret 2006
        </timeline-time>
        <timeline-title>
          Kelahiran
        </timeline-title>
        <timeline-body>
          Momen bahagia dan tak akan pernah terlupakan saya Al-farizy M G telah terlahir di dunia ini. Keluarga berbahagia kerabat bersyukur ria.
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time style="color:darkcyan;">
           2013
        </timeline-time>
        <timeline-title>
          Awal Pendidikan
        </timeline-title>
        <timeline-body>
          Saya bersekolah dimanapaun orang tua saya menempatkan saya untuk bersekolah. Saya tak pernah semangat ketika pergi bersekolah. Berangkat dengan sangat rapih dan datang amat awal pagi, hanya untuk menyempatkan diri untuk tidur sebentar di sekolah.
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time style="color:darkcyan;">
          juli 2018
        </timeline-time>
        <timeline-title>
          Awal mula SMP
        </timeline-title>
        <timeline-body>
          Saya melanjutkan sekolah smp dengan melalui jalur zonasi, karna dulu saya masih bego. untungnya jarak antara rumah saya dan sekolah tidak terlalu jauh. Naas Lockdown harus terjadi akibat covid-19 yang menerjang dunia.
        </timeline-body>
      </timeline-content>
      </timeline-item>
      <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time style="color:darkcyan;">
          juli 2021
        </timeline-time>
        <timeline-title>
          Awal mula SMK
        </timeline-title>
        <timeline-body>
           Saya masuk SMK dengan memilih jurusan RPL. Ditengah-tengah covid-19 kita saya dengan malasnya tetap harus menempuh ilmu karna itu adalah kewajiban saya sebagai seorang manusia.  
        </timeline-body>
      </timeline-content>
      </timeline-item>
      <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time style="color:darkcyan;">
          Pertengahan Tahun 2024
        </timeline-time>
        <timeline-title>
          Akan menjadi seperti apakah saya <h2>?</h2>
        </timeline-title>
        <timeline-body>
          ...
        </timeline-body>
      </timeline-content>
    </timeline-item>
  </Timeline>
</div>

<Progress progress="100" class="my-5" style="margin: 5px;"></Progress>

<div class="flex" id="about">
    <the-card href="#" class="my-5" style="background-color: steelblue; margin: 20px;">
    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Tentang Saya</h5>
    <p class="font-normal text-gray-700 dark:text-gray-400">
      Saya bersekolah di salah satu SMK Pusat Terpadu. Selama bersekolah di SMK saya mengambil jurusan RPL(Rekayasa Perangkat Lunak), di sini saya diajarkan berbagai macam bahasa pemrograman. Karena itulah saya cukup mahir dan bisa dalam menguasai beberapa bahasa pemrograman. Oleh karena itu pula kemampuan saya akan amat sangat di butuhkan salam dunia digital pada saat ini.
    </p>
  </the-card>

 <div class="my-5" id="talenta">
    <h6 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Talenta kemampuan</h6>
    <Progress labelProgress="true" color="red" label="HTML" labelPosition="outside" size="sm" progress="45" style="width: 750px;"></Progress>
  <Progress labelProgress="true" color="yellow" label="CSS" labelPosition="outside" size="sm" progress="45" style="width: 750px;"></Progress>
  <Progress labelProgress="true" color="yellow" label="JavaScript" labelPosition="outside" size="sm" progress="45" style="width: 750px;"></Progress>
  <Progress labelProgress="true" color="green" label="Node.JS" labelPosition="outside" size="sm" progress="45" style="width: 750px;"></Progress>
  <Progress labelProgress="true" color="green" label="Vue.JS" labelPosition="outside" size="sm" progress="45" style="width: 750px;"></Progress>
  <Progress labelProgress="true" color="purple" label="UI/UX" labelPosition="outside" size="sm" progress="100" style="width: 750px;"></Progress>
 </div>
</div>

<Progress progress="100" class="mt-5" style="margin: 5px;"></Progress>

<div class="flex item-center ">
<div class="max-w-lg rounded-lg shadow-md shadow-blue-600/50 my-5 flex item-center w-full mx-auto max-w-screen-xl p-4 md:flex md:items-center md:justify-between" style="background-color:steelblue; margin: 20px;" >
    <div class="w-full p-4">
        <label for="username-success" class=" mb-2 text-sm font-medium text-gray-900 dark:text-white" >Your Name</label>
<input type="username-success" id="username-success" aria-describedby="helper-text-explanation" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="your name">

<label for="email" class=" mb-2 text-sm font-medium text-gray-900 dark:text-white">Your email</label>
<input type="email" id="email" aria-describedby="helper-text-explanation" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5  dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="name@gmail.com">
    </div>

  <form class="w-full p-4">
    <div class="mb-2 mt-6">
      <label for="comment" class="mb-2 text-sm font-medium text-gray-900 dark:text-white">Add a comment</label>
      <textarea
        class="w-full h-20 p-2 border rounded focus:outline-none focus:ring-gray-300 focus:ring-1"
        name="comment"
        placeholder=""></textarea>
    </div>
    <div>
      <button class="px-3 py-2 text-sm text-blue-100 bg-blue-600 rounded">
        Comment
      </button>
      <button
        class="px-3 py-2 text-sm text-blue-100 bg-blue-600 border border-blue-500 rounded">
        Cancel
      </button>
    </div>
  </form>
</div>
</div>


<div id="social-platforms">
<a class="btn btn-icon btn-facebook" href=""><i class="fa fa-facebook"></i><span>Facebook</span></a>
<a class="btn btn-icon btn-instagram" href="#"><i class="fa fa-instagram"></i><span>Instagram</span></a>
<a class="btn btn-icon btn-github" href="https://github.com/alfarizymourinho"><i class="fa fa-github"></i><span>Github</span></a>
</div>


<footer class="rounded-lg shadow m-4 dark:bg-gray-800">
    <div class="w-full mx-auto max-w-screen-xl p-4 md:flex bg-gray-800 md:items-center md:justify-between">
      <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2023 <a href="https://flowbite.com/" class="hover:underline">Al-farizy M G™</a>. All Rights Reserved.
    </span>
    <ul class="flex flex-wrap items-center mt-3 text-sm font-medium text-gray-500 dark:text-gray-400 sm:mt-0">
        <li>
            <a href="#" class="mr-4 hover:underline md:mr-6 ">About</a>
        </li>
        <li>
            <a href="#" class="mr-4 hover:underline md:mr-6">Privacy Policy</a>
        </li>
        <li>
            <a href="#" class="mr-4 hover:underline md:mr-6">Licensing</a>
        </li>
        <li>
            <a href="#" class="hover:underline">Contact</a>
        </li>
    </ul>
    </div>
</footer>


</template>
