<script>
  import { Container, Image, Row, Col } from "sveltestrap";
  import Calendar from "$lib/Calendar.svelte";
</script>

<div class="bg-light border-bottom">
  <Container class="col-xxl-8 px-4 py-5">
    <Row class="flex-lg-row-reverse align-items-center g-5 py-2">
      <Col xs="10" sm="8" lg="6">
        <Image fluid src="home.png" />
      </Col>
      <Col lg="6">
        <h1 class="display-5 fw-bold">BIENVENIDO A AULAPLAN</h1>
        <p class="lead">
          Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint
          cillum sint consectetur cupidatat.
        </p>
      </Col>
    </Row>
  </Container>
</div>

<Calendar />

