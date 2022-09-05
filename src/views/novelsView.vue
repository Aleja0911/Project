<template>
    <body>
        <h1>Novelas</h1>
        <main class="books">
            <div class="book1">
                <img src="" alt="libro1">
            </div>
            <div class="text1">
                <p>La primera novela de Mario Mendoza es
                 un descenso a los abismos de Bogotá para
                 hablar de personajes con los que nadie
                 se quiere meter. Como un beligerante
                 escritor del realismo francés del siglo
                 XIX, Mendoza narra la soledad de seres
                 que un día se quedaron al margen de
                 todo, abandonados a su desesperación y
                 su locura.</p>
            </div>

            <div class="book2">
                <img src="" alt="Libro2">
            </div>
            <div class="text2">
                <p>Una novela sobre la oscura presencia
                de lo maligno en la vida cotidiana. Una
                mujer hermosa e ingenua que roba con
                destreza a altos ejecutivos, un pintor
                habitado por fuerzas misteriosas, y un
                sacerdote que se enfrenta a un caso de
                posesión demoníaca en La Candelaria, el
                barrio colonial de Bogotá…historias que
                se tejen en torno a la de Campo Elías,
                héroe de la guerra de Vietnam, quien
                inicia su particular descenso a los
                infiernos obsesionado por la dualidad
                entre elbien y el mal, entre Jekyll y
                Hyde, y se convertirá en un ángel
                exterminador</p>
            </div>

            <div class="book3">
                <img src="" alt="libro3">
            </div>
            <div class="text3">
                <p>Un hombre, Tafur, está en prisión.
                Trata de reconstruir su vida a través de
                sus memorias para llegar a entender qué
                lo llevó a cometer un cruel asesinato.
                Con una prosa que cautiva desde el
                comienzo, Mario Mendoza sumerge al lector
                en la ambivalente vida de un individuo
                que busca liberarse de sus obsesiones.</p>
            </div>

            <div class="book4">
                <img src="" alt="libro4">
            </div>
            <div class="text4">
                <p>Un imitador de Jack el Destripador
                está inmerso en una auténtica orgía de
                sangre y mata prostitutas sin
                contemplación. Mientras Molina sigue
                pistas de un extremo a otro de la capital
                para dar con el criminal, sus pasos se
                cruzan con los de su mentor, un sacerdote
                atormentado por los secretos que esconde
                de su juventud.</p>
            </div>

            <div class="book5">
                <img src="" alt="libro5">
            </div>
            <div class="text5">
                <p>A los siete años, mientras le hacía el
                    quite a la muerte en una cama de
                    hospital, Mario Mendoza descubrió los
                    libros y su potencia liberadora con
                    un ejemplar de Cuentos de hadas
                    franceses. En ese momento se volvió
                    lector e inició una amistad
                    inquebrantable con aquellos objetos.
                    “Seguiremos leyendo porque las
                    páginas que amamos, en medio del
                    infierno que vivimos día a día, son
                    nuestra única redención posible”.</p>
            </div>

            <div class="book6">
                <img src="" alt="libro6">
            </div>
            <div class="text6">
                <p>Diez historias colombianas sobre el
                vidente que salvó al mejor amigo de un
                presidente, pero que después se quedó
                solo; sobre el preso travestido que habla
                con extraterrestres; sobre la mujer que
                fue poseída por el espíritu de Manuelita
                Sáenz y vio a Simón Bolívar a los ojos.</p>
            </div>
        </main>
    </body>
</template>

<style>
.book1{
    grid-area: a;
}
.book2{
    grid-area: b;
}
.book3{
    grid-area: c;
}
.book4{
    grid-area: d;
}
.book5{
    grid-area: e;
}
.book6{
    grid-area: f;
}
/* textosss */
.text1{
    grid-area: g;
}
.text2{
    grid-area: h;
}
.text3{
    grid-area: i;
}
.text4{
    grid-area: j;
}
.text5{
    grid-area: k;
}
.text6{
    grid-area: l;
}
.books{
    display: grid;
    grid-template:
    "a"
    "g"
    "b"
    "h"
    "c"
    "i"
    "d"
    "j"
    "e"
    "k"
    "f"
    "l";
}

@media (min-width: 600px) {
    .books{
        grid-template:
        "a g"
        "b h"
        "c i"
        "d j"
        "e k"
        "f l";
    }
}
@media (min-width: 900px) {
    .books{
        grid-template:
        "a g"
        "b h"
        "c i"
        "d j"
        "e k"
        "f l";
    }
}
</style>
