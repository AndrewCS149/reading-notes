# View Components 

### What are View Components?

View components are similar to partial views but have more functionality. View components are typically used over partial views when:

- Heavier business logic is involved
- Navigation menus
- Logins
- Shopping carts
- Recently published articles

View Components have two parts:

- The Class
- The result (normally a view)

---

### Search path

`/Pages/Shared/Components/{view component name}/{view name}`

---

### Invoking a View Component

`@await Component.InvokeAsync("Name of view component", {Anonymous Type Containing Parameters}) `


