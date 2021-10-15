<script>
    import {
        Collapse,
        Navbar,
        NavbarToggler,
        NavbarBrand,
        Nav,
        NavItem,
        NavLink,
        UncontrolledDropdown,
        DropdownToggle,
        DropdownMenu,
        DropdownItem,
        Button,
    } from "sveltestrap";

    let isOpen = false;

    function handleUpdate(event) {
        isOpen = event.detail.isOpen;
    }
</script>

<Navbar color="primary" dark expand="md" class="fixed-top">
    <NavbarBrand href="/" class="text-uppercase ">Educate App</NavbarBrand>
    <NavbarToggler on:click={() => (isOpen = !isOpen)} />
    <Collapse {isOpen} navbar expand="md" on:update={handleUpdate}>
        <Nav class="ml-auto mr-5 py-2" navbar>
            <NavItem class="ml-4 text-uppercase active">
                <NavLink href="#!">Home</NavLink>
            </NavItem>
            <NavItem class="ml-4 text-uppercase">
                <NavLink href="#!">Our Work</NavLink>
            </NavItem>
            <NavItem class="ml-4 text-uppercase">
                <NavLink href="#!">Product</NavLink>
            </NavItem>
            <NavItem class="ml-4 text-uppercase">
                <NavLink href="#!">Blog</NavLink>
            </NavItem>
            <NavItem class="ml-4 text-uppercase">
                <NavLink href="#!">Contact Us</NavLink>
            </NavItem>

            <a href="#!" class="btn btn-default ml-4 text-uppercase buttonStyle"
                >Login</a
            >
        </Nav>
    </Collapse>
</Navbar>

<style>
    .buttonStyle {
        border-radius: 20px;
        background-color: orange;
        color: white;
    }
    .buttonStyle:hover {
        border-radius: 20px;
        background-color: orange;
        color: white;
    }
</style>
