# Development

NOTE: Overall design/idea of website was previously developed for the responsive redesign project. However, actual development of this project is completely different as all buttons and functionality of that project were dummies and the data was hard-coded into the front-end.

### Link to Deployed Website

`https://delightfuldolphin212.github.io/development`

### Goal and Value of the Application

Goal is to provide an innovative interface through which customers can visually see the contents of the FineWineCollector online wine shop and add filter through/add available wines to their carts

### Usability Principles Considered

For usability text size, contrast, and responsiveness.

For readibility and code style, paid close attention to hierarchy of the app, creating components for not only store and cart items, but also the SidePane which controls sorting and filtering. I plan on developing this project into my capstone and am prepared to create more components for elements such as a navigation bar along the top.

### Organization of Components

Individual components for WineItem, CartItem, and the SidePane which contains the sort/filter options

WineItem is dependent on props including the actual item being rendered, as well as the two state variables and their setters which keep track of the current contents of the cart as well as the total price of the cart.

CartItem uses identical props except it also leverages the index number of the current item in the list being mapped.

Lastly, the SidePane component uses props for WineData, which is the original raw data, as well as the state variable representing the current items to be displayed in the store and its setter (used for filtering/sorting).

### How Data is Passed Down Through Components

Data is passed through props through the components in the form of state variables which are used and updated throughout the components

### How the User Triggers State Changes

State changes are triggered by the add to cart button as well as the remove from cart button, both of which edit the cart contents state variable. Other various state variables are used throughout to manage other parts of the application including which filters are active and not active to make the SidePane responsive (buttons activate and deactivate)
