# VAutocomplete Infinite Scroll Component

This repository provides a Vue 3 component using Vuetify 3 that extends the VAutocomplete functionality with infinite scrolling capabilities. The component allows users to search for and select items from a dynamically loaded list, ideal for applications with large datasets where loading all items at once is impractical.

## Features

- **Infinite Scrolling**: As users scroll, additional data is fetched and appended to the list, ensuring smooth and continuous scrolling.
- **Dynamic Search**: The component updates the search results in real time based on user input.
- **Loading Indicators**: Visual feedback is provided to inform users when more data is being loaded or when all data has been loaded.
- **Intersection Observer**: Efficient data fetching is achieved using the Intersection Observer API to detect when the user reaches the end of the list.
- **Clearable Selection**: Users can easily clear their selection, resetting the search and list state.

## Installation

To integrate this component into your project, follow these steps:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/YoussefAMansour/VAutocomplete-Infinite-Scroll-Single-Select
   
2. **Navigate to the project directory**:
    ```sh
   cd v-autocomplete-infinite-scroll

3.  **Install dependencies**:
    ```sh
    npm install
4.  **Run the project**:
    ```sh
    npm run serve

## Usage

Here's an example of how to use the VAutocomplete Infinite Scroll component in your Vue 3 application:
1. ```shell
    <template>
        <div>
        <VAutocompleteInfiniteScroll />
      </div>
    </template>

    <script setup>
        import VAutocompleteInfiniteScroll from '@/components/VAutocompleteInfiniteScroll.vue';
    </scrpit>

## Configuration

The component can be customized through several props and slots:

Props:
* items: Array of items to be displayed in the autocomplete.
* item-text: Property name to display in the list.
* item-value: Property name to use as the value.
* label: Label for the autocomplete input.
* search-input.sync: Two-way binding for the search input.
* return-object: Boolean to return the full object instead of just the value.
* clearable: Boolean to enable clearing the selection.
* autocomplete: Attribute to disable browser autocomplete.


Slots:
* append-item: Custom content to append at the end of the list, typically used for loading indicators


## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request if you have any ideas, suggestions, or improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
