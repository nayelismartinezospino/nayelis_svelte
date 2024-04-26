<script>
    export let pais;
    let p;
    /*[0]=nombre_pais [1]=capital [2]=poblacion [3]=moneda [4]=area [5]=bandera*/
    const paises = {
        Colombia: [
            "Colombia",
            "Bogota",
            "51,2 millones",
            "pesos colombianos",
            "1,142 millones km2",
            "colombia.jpg",
        ],
        Venezuela: [
            "Venezuela",
            "Caracas",
            "28,2 millones",
            "bolivar",
            "916.445 km2",
            "venezuela.jpg",
        ],
        Ecuador: [
            "Ecuador",
            "Quito",
            "17,8 millones",
            "dolar estadunidense",
            "256.370 km2",
            "ecuador.jpg",
        ],
        Peru: [
            "Peru",
            "Lima",
            "33,72 millones",
            "sol peruano",
            "1.285.215 km2",
            "peru.jpg",
        ],
        Brasil: [
            "Brasil",
            "Brasilia",
            "214,3 millones",
            "real brasileño",
            "8,51 km2",
            "brasil.jpg",
        ],
        Paraguay: [
            "Paraguay",
            "Asuncion",
            "6.109.644 millones",
            "guarani",
            "15,02 km2",
            "paraguay.jpg",
        ],
        Bolivia: [
            "Bolivia",
            "Sucre",
            "12.186.073 millones",
            "boliviano",
            "11,09 km2",
            "bolivia.jpg",
        ],
        Uruguay: [
            "Uruguay",
            "Montevideo",
            "3,444,263 millones",
            "uruguayan peso",
            "19.5 km2",
            "uruguay.jpg",
        ],
        Argentina: [
            "argentina",
            "buenos aires",
            "4,444,263 millones",
            "peso argentino",
            "2.78 km2",
            "Argentina.jpg",
        ],
        Chile: [
            "chile",
            "santiago",
            "2,423,263 millones",
            "peso chileno",
            "756.626 km2",
            "chile.jpg",
        ],
    };
    p = paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img
            src="./src/assets/{p[5]}"
            alt="Bandera_Colombia"
            width="300"
            height="200"
        />
    </div>
    <div class="col2">
        <div class="linea"><strong>Pais:</strong>{p[0]}</div>
        <div class="linea"><strong>Capital:</strong>{p[1]}</div>
        <div class="linea"><strong>Poblacion:</strong>{p[2]}</div>
        <div class="linea"><strong>Moneda:</strong>{p[3]}</div>
        <div class="linea"><strong>Extension:</strong>{p[4]}</div>
    </div>
</div>

<style>
    .main {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-gap: 40px;
        grid-auto-rows: minmax(100px, auto);
        border-radius: 30px;
        font-family: "Trebuchet MS", "Lucida Sans Unicode", "Lucida Grande",
            "Lucida Sans", Arial, sans-serif;
        border-style: double;
        border-color: rgb(14, 13, 13);
        border-width: 7px;
        margin: left;
        width: 750px;
        box-shadow: 9px 20px 20px rgb(36, 33, 211);
        margin-right: 20px;
        margin-bottom: 20px;
    }
    .col1 {
        grid-column: 3;
        grid-row: 1;
        margin: 19px;
        padding: 22px;
    }
    .col2 {
        grid-column: 2;
        grid-row: 1;
        margin: 9x;
        padding: 10px;
        border-color: black;
        width: max-content;
    }
    strong {
        color: rgb(0, 0, 0);
        font-weight: bolder;
    }
    .linea {
        font-size: 19px;
        margin-bottom: 22px;
        font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    }
</style>
