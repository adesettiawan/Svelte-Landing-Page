<script>
    import { Col, Row } from "sveltestrap";

    let _tahun = new Date().getFullYear();
</script>

<footer class="bg-primary text-white text-lg-start">
    <!-- Grid container -->
    <div class="container-fluid py-5">
        <!--Grid row-->
        <Row>
            <!--Grid column-->
            <Col xl="6" xs="12">
                <h5 class="text-uppercase">Footer Content</h5>

                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Iste atque ea quis molestias. Fugiat pariatur maxime quis
                    culpa corporis vitae repudiandae aliquam voluptatem veniam,
                    est atque cumque eum delectus sint!
                </p>
            </Col>
            <!--Grid column-->

            <!--Grid column-->
            <Col xl="3" xs="6">
                <h5 class="text-uppercase">Links</h5>

                <ul class="list-unstyled mb-0">
                    <li>
                        <a href="#!" class="text-white">Link 1</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Link 2</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Link 3</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Link 4</a>
                    </li>
                </ul>
            </Col>
            <!--Grid column-->

            <!--Grid column-->
            <Col xl="3" xs="6">
                <h5 class="text-uppercase">Links</h5>

                <ul class="list-unstyled  mb-0">
                    <li>
                        <a href="#!" class="text-white">Link 1</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Link 2</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Link 3</a>
                    </li>
                    <li>
                        <a href="#!" class="text-white">Link 4</a>
                    </li>
                </ul>
            </Col>
            <!--Grid column-->
        </Row>
        <!--Grid row-->
    </div>
    <!-- Grid container -->

    <!-- Copyright -->
    <div class="text-center p-3 footerStyle">
        © {_tahun} Latihan:
        <a class="text-white" href="https://svelte.dev/">Svelte.dev</a>
    </div>
    <!-- Copyright -->
</footer>

<style>
    .footerStyle {
        background-color: rgba(0, 0, 0, 0.2);
    }
</style>
