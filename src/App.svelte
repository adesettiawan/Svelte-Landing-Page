<script>
    import { Col, Row, Media } from "sveltestrap";
    import Card from "./Card/Card.svelte";
    import Carousel from "./Carousel/Carousel.svelte";
    import Footer from "./Footer/Footer.svelte";
    import NavigatorBar from "./Navbar/NavigatorBar.svelte";
</script>

<main>
    <NavigatorBar />
    <Carousel />
    <div class="container mt-5">
        <Row>
            <Col xs="6"><img src="../img/humans.png" alt="Gambar 1" /></Col>
            <Col xs="6">
                <div class="aStyle">
                    <h5 class="tittleStyle">
                        <strong> Why <br /> Educate</strong>
                        <span class="firstStyle"><b>First</b></span> ?
                    </h5>
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing
                        elit. Rem expedita, neque nihil eius et assumenda!
                        Libero vero magnam cumque voluptatum aut, commodi
                        tenetur maxime incidunt fuga ea asperiores ab autem!
                    </p>
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing
                        elit. Sit deleniti tempora amet excepturi ratione dolor
                        ducimus voluptatibus, quis possimus commodi molestiae
                        aspernatur.
                    </p>
                    <a href="#!" class="text-danger">Learn More!</a>
                </div>
            </Col>
        </Row>
    </div>

    <div class="container mt-5 mb-5">
        <Row>
            <Col xs="6">
                <div class="bStyle">
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing
                        elit. Rem expedita, neque nihil eius et assumenda!
                        Libero vero magnam cumque voluptatum aut, commodi
                        tenetur maxime incidunt fuga ea asperiores ab autem!
                    </p>
                </div>
            </Col>
            <Col xs="6"
                ><img
                    class="humansOne"
                    src="../img/humans1.png"
                    alt="Gambar 1"
                /></Col
            >
        </Row>
    </div>

    <div class="container mt-5 mb-5">
        <Row>
            <Col xs="8"
                ><Media>
                    <Media left href="#">
                        <Media
                            object
                            src="/icon/pemateri.svg"
                            class="align-self-center"
                            alt="Generic placeholder image"
                        />
                    </Media>
                    <Media body class="ml-3">
                        <Media heading>Pemateri</Media>
                        Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
                        scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum
                        in vulputate at, tempus viverra turpis. Fusce condimentum
                        nunc ac nisi vulputate fringilla. Donec lacinia congue felis
                        in faucibus.
                    </Media>
                </Media></Col
            >
            <Col xs="4"><Card /></Col>
            <Col xs="8"
                ><Media>
                    <Media left href="#">
                        <Media
                            object
                            src="/icon/mitra.svg"
                            class="align-self-center"
                            alt="Generic placeholder image"
                        />
                    </Media>
                    <Media body class="ml-3">
                        <Media heading>Kemitraan</Media>
                        Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
                        scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum
                        in vulputate at, tempus viverra turpis. Fusce condimentum
                        nunc ac nisi vulputate fringilla. Donec lacinia congue felis
                        in faucibus.
                    </Media>
                </Media></Col
            >
            <Col xs="4"><Card /></Col>
            <Col xs="8"
                ><Media>
                    <Media left href="#">
                        <Media
                            object
                            src="/icon/talks.svg"
                            class="align-self-center"
                            alt="Generic placeholder image"
                        />
                    </Media>
                    <Media body class="ml-3">
                        <Media heading>Talks/Webinar</Media>
                        Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
                        scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum
                        in vulputate at, tempus viverra turpis. Fusce condimentum
                        nunc ac nisi vulputate fringilla. Donec lacinia congue felis
                        in faucibus.
                    </Media>
                </Media></Col
            >
            <Col xs="4"><Card /></Col>
            <Col xs="8"
                ><Media>
                    <Media left href="#">
                        <Media
                            object
                            src="/icon/peta.svg"
                            class="align-self-center"
                            alt="Generic placeholder image"
                        />
                    </Media>
                    <Media body class="ml-3">
                        <Media heading>Relasi</Media>
                        Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
                        scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum
                        in vulputate at, tempus viverra turpis. Fusce condimentum
                        nunc ac nisi vulputate fringilla. Donec lacinia congue felis
                        in faucibus.
                    </Media>
                </Media></Col
            >
            <Col xs="4"><Card /></Col>
        </Row>
    </div>

    <Footer />
</main>

<style>
    .aStyle {
        margin-top: 45px;
    }
    .bStyle {
        margin-top: 90px;
    }
    .tittleStyle {
        font-size: 45px;
    }
    .firstStyle {
        color: darkcyan;
        font-size: 50px;
    }
    .humansOne {
        margin-left: 90px;
        width: 450px;
        height: 350px;
    }
</style>
