class BarraMovel {
    constructor(menuBoton, naveLista, naveLinks){
        this.menuBoton = document.querySelector(menuBoton);
        this.naveLista = document.querySelector(naveLista);
        this.naveLinks = document.querySelectorAll(naveLinks);
        this.classeAtiva = "active";
        this.handleClick = this.handleClick.bind(this);
    }

    animaLinks(){
        this.naveLinks.forEach((link) => {
            link.style.animation
            ? (link.style.animation ="")
            : (link.style.animation = 'naveLinkFade 0.4s ease forwards 0.25s');
        });
    }

    handleClick (){
        this.naveLista.classList.toggle(this.classeAtiva);
        this.menuBoton.classList.toggle(this.classeAtiva);
        this.animaLinks();
    }

    addClickEvent (){
        this.menuBoton.addEventListener("click", this.handleClick);
    }

    init() {
        if (this.menuBoton){
            this.addClickEvent();
        }
        return this;
    }
}
    const barraMovel = new BarraMovel(
        ".menu-movel",
        ".nave-lista",
        ".nave-lista li",
);
barraMovel.init();
