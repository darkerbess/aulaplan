<script>
  import {
    NavItem,
    Navbar,
    NavbarBrand,
    Nav,
    Button,
    Container,
    FormGroup,
    Input,
  } from "sveltestrap";
</script>

<Navbar light expand="md" class="border-bottom py-md-4">
  <Container class="d-flex">
    <NavbarBrand class="me-auto" href="/">AulaPlan</NavbarBrand>
    <div class="vr ms-2" />
    <Container>
      <FormGroup class="mb-auto">
        <!-- TODO: Icon for search input  -->
        <Input
          type="search"
          name="search"
          placeholder="Type to search"
          class="border-0 shadow-none"
        />
      </FormGroup>
    </Container>
    <Nav navbar>
      <NavItem>
        <!-- TODO: Icon for login button  -->
        <Button color="primary">Login</Button>
      </NavItem>
    </Nav>
  </Container>
</Navbar>

<!-- TODO: Collapse for Search Input -->
