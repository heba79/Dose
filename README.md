<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1">

<head>
    <style>
        .a {
            font-size: xx-large;
            font-style: italic;
            color: #0e9bba;
        }

        *::after,
        *::before {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        .container {
            width: 70%;
            margin: 4rem auto;
            position: relative;

        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(8, 1fr);
            grid-template-rows: repeat(8, 5vw);
            grid-gap: 1rem;
        }

        .gallery__img {
            width: 150px;
            height: 150px;
            object-fit:fill;
            border-radius: 8px;

        }

        .gallery__item--1 {
            grid-column-start: 1;
            grid-column-end: 3;
            grid-row-start: 1;
            grid-row-end: 3;
            color: white;

        }

        .gallery__item--2 {
            grid-column-start: 3;
            grid-column-end: 6;
            grid-row-start: 1;
            grid-row-end: 3;


        }

        .gallery__item--3 {
            grid-column-start: 5;
            grid-column-end: 7;
            grid-row-start: 1;
            grid-row-end: 3;


        }

        .gallery__item--4 {
            grid-column-start: 7;
            grid-column-end: 9;
            grid-row-start: 1;
            grid-row-end: 3;

        }

        .gallery__item--5 {
            grid-column-start: 10;
            grid-column-end: 12;
            grid-row-start: 1;
            grid-row-end: 3;

        }

        .gallery__item--6 {
            grid-column-start: 1;
            grid-column-end: 3;
            grid-row-start: 3;
            grid-row-end: 5;
        }

        .gallery__item--7 {
            grid-column-start: 3;
            grid-column-end: 6;
            grid-row-start: 3;
            grid-row-end: 5;
        }

        .gallery__item--8 {
            grid-column-start: 5;
            grid-column-end: 7;
            grid-row-start: 3;
            grid-row-end: 5;
        }

        .gallery__item--9 {
            grid-column-start: 7;
            grid-column-end: 9;
            grid-row-start: 3;
            grid-row-end: 5;
        }

        .gallery__item--10 {
            grid-column-start: 10;
            grid-column-end: 12;
            grid-row-start: 3;
            grid-row-end: 5;
        }

        .overlay {
            position: absolute;
            height: 150px;
            width: 150px;
            opacity: 0;
            transition: .5s ease;
            background-color: #0e9bba;
            color: white;
        }

        .text {
            color: rgb(251, 248, 248);
            font-size: 20px;
            position: absolute;
            top: 50%;
            left: 50%;
            -webkit-transform: translate(-50%, -50%);
            -ms-transform: translate(-50%, -50%);
            transform: translate(-50%, -50%);
            text-align: center;
            position: absolute;
        }

        .btn {
            border: none;
            text-align: center;
            font-size: 16px;
            opacity: 1;
            display: inline-flex;
            cursor: pointer;
            width: 150px;
            height: 150px;
            border-radius: 8px;


        }

        .btn:hover .overlay {
            opacity: 1;
            font-size: 20px;
            border-radius: 8px;
        }
      
    </style>
</head>

<body>
    <div class="a">Categories</div>
    <div class="container">
        <div class="gallery">
            <figure class=" gallery__item--1">
                <button class="btn">                  
                    <img src="medicationsedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Medications</div>

                    </div>
                </button>
            </figure>
            <figure class=" gallery__item--2">
                <button class="btn">
                    <img src="vitaminsedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Vitamins</div>
                    </div>
                </button>
            </figure>
            <figure class="gallery__item--3">
                <button class="btn">
                    <img src="Bodypersonalcareedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Personal Care</div>
                    </div>
                </button>
            </figure>




            <figure class=" gallery__item--4">
                <button class="btn">
                    <img src="makeupedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Beauty Products</div>
                    </div>
                </button>
            </figure>

            <figure class=" gallery__item--5">
                <button class="btn">
                    <img src="skincareedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Skin Care</div>
                    </div>
                </button>
            </figure>
            <figure class=" gallery__item--6">
                <button class="btn">
                    <img src="cleaningproductsedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Cleaning products</div>
                    </div>
                </button>
            </figure>
            <figure class=" gallery__item--7">
                <button class="btn">
                    <img src="motherbabycareedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Mother/Baby Care</div>
                    </div>
                </button>
            </figure>
            <figure class=" gallery__item--8">
                <button class="btn">
                    <img src="medicalsuppliesedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Medical Suplments</div>
                    </div>
                </button>
            </figure>
            <figure class=" gallery__item--9">
                <button class="btn">

                    <img src="haircareedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Hair Care</div>
                    </div>
                </button>
            </figure>
            <figure class=" gallery__item--10">
                <button class="btn">
                    <img src="perfumesedited.jpg" class="gallery__img">
                    <div class="overlay">
                        <div class="text">Perfumes</div>
                    </div>
                </button>
            </figure>
        </div>
    </div>
</body>

</html>