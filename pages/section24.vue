<template>
<div class="carousel relative max-w-md rounded-xl container mx-2 border border-gray-200 shadow-md" style="max-width:1600px;">
        <div class="carousel-inner relative overflow-hidden w-full rounded-2xl">
            <!--Slide 1-->
            <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
            <div class="carousel-item absolute opacity-0" style="height:100vh;">
                <div class="block h-full w-full mx-auto flex pt-6 md:pt-0 md:items-center bg-cover bg-right " >
                <img src="../static/s23.png" alt="">
                </div>
            </div>
            <label for="carousel-3" class="prev control-1 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-gray-900 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
            <label for="carousel-2" class="next control-1 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-gray-900 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>

            <!--Slide 2-->
            <input class="carousel-open" type="radio" id="carousel-2" name="carousel" aria-hidden="true" hidden="">
            <div class="carousel-item absolute opacity-0 bg-cover bg-right" style="height:100vh;">
                <div class="block h-full w-full mx-auto flex pt-6 md:pt-0 md:items-center bg-cover bg-right " >
                <img src="../static/section23.png" alt="">
                </div>
            </div>
            <label for="carousel-1" class="prev control-2 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-gray-900  leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
            <label for="carousel-3" class="next control-2 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-gray-900  leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>

            <!--Slide 3-->
            <input class="carousel-open" type="radio" id="carousel-3" name="carousel" aria-hidden="true" hidden="">
                <div class="carousel-item absolute opacity-0 bg-cover bg-right" style="height:100vh;">
                 <div class="block h-full w-full mx-auto flex pt-6 md:pt-0 md:items-center bg-cover bg-right " >
                <img src="../static/s24.png" alt="">
                </div>
            </div>
            <label for="carousel-2" class="prev control-3 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-gray-900  leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
            <label for="carousel-1" class="next control-3 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-gray-900  leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>

            <!-- Add additional indicators for each slide
            <ol class="carousel-indicators">
                <li class="inline-block mr-3">
                    <label for="carousel-1" class="carousel-bullet cursor-pointer block text-4xl text-gray-400 hover:text-gray-900">•</label>
                </li>
                <li class="inline-block mr-3">
                    <label for="carousel-2" class="carousel-bullet cursor-pointer block text-4xl text-gray-400 hover:text-gray-900">•</label>
                </li>
                <li class="inline-block mr-3">
                    <label for="carousel-3" class="carousel-bullet cursor-pointer block text-4xl text-gray-400 hover:text-gray-900">•</label>
                </li>
            </ol> -->
                <div class="p-5">
        <a href="#">
            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Section 24 Understanding GraphQL Mutation</h5>
        </a>
        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
            Resume Section 24 GraphQL Mutation

            Sebagian besar diskusi GraphQL berfokus pada pengambilan data, tetapi semua platform data lengkap memerlukan cara untuk memodifikasi data sisi server juga.

            Di REST, permintaan apa pun mungkin berakhir menyebabkan beberapa efek samping pada server, tetapi menurut konvensi, disarankan agar seseorang tidak menggunakan permintaan GET untuk mengubah data. GraphQL serupa - secara teknis kueri apa pun dapat diimplementasikan untuk menyebabkan penulisan data. Namun, berguna untuk menetapkan konvensi bahwa setiap operasi yang menyebabkan penulisan harus dikirim secara eksplisit melalui mutasi.

            Sama seperti dalam kueri, jika bidang mutasi mengembalikan tipe objek, Anda dapat meminta bidang bersarang. Ini dapat berguna untuk mengambil status baru suatu objek setelah pembaruan.

            Mutasi dapat berisi beberapa bidang, seperti kueri. Ada satu perbedaan penting antara kueri dan mutasi, selain namanya:

            Sementara bidang kueri dijalankan secara paralel, bidang mutasi dijalankan secara seri, satu demi satu.

            Ini berarti bahwa jika kita mengirim dua mutasi incrementCredits dalam satu permintaan, yang pertama dijamin selesai sebelum yang kedua dimulai, memastikan bahwa kita tidak berakhir dengan kondisi balapan dengan diri kita sendiri.
        </p>
    </div>
    </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
  .work-sans {
            font-family: 'Work Sans', sans-serif;
        }
                
        #menu-toggle:checked + #menu {
            display: block;
        }
        
        .hover\:grow {
            transition: all 0.3s;
            transform: scale(1);
        }
        
        .hover\:grow:hover {
            transform: scale(1.02);
        }
        
        .carousel-open:checked + .carousel-item {
            position: static;
            opacity: 100;
        }
        
        .carousel-item {
            -webkit-transition: opacity 0.6s ease-out;
            transition: opacity 0.6s ease-out;
        }
        
        #carousel-1:checked ~ .control-1,
        #carousel-2:checked ~ .control-2,
        #carousel-3:checked ~ .control-3 {
            display: block;
        }
        
        .carousel-indicators {
            list-style: none;
            margin: 0;
            padding: 0;
            position: absolute;
            bottom: 2%;
            left: 0;
            right: 0;
            text-align: center;
            z-index: 10;
        }
        
        #carousel-1:checked ~ .control-1 ~ .carousel-indicators li:nth-child(1) .carousel-bullet,
        #carousel-2:checked ~ .control-2 ~ .carousel-indicators li:nth-child(2) .carousel-bullet,
        #carousel-3:checked ~ .control-3 ~ .carousel-indicators li:nth-child(3) .carousel-bullet {
            color: #000;
            /*Set to match the Tailwind colour you want the active one to be */
        }
</style>