**react-native-easy-carousel**

A simple and easy-to-use carousel component for React Native, designed to provide a smooth and customizable experience for displaying content in a horizontal scrollable view.

**Features**

- Easy Integration: Simple API to integrate the carousel into your React Native projects.
- Autoplay: Supports automatic scrolling with a customizable interval.
- Index Change Handling: Provides a callback for index change events.
- Customizable: Easily customize the appearance and behavior of the carousel and its items.
- Responsive: Automatically adjusts to the screen size for a seamless user experience.

**Installation**

Install the package using npm:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  javaCopy codenpm install react-native-easy-carousel  `

**Usage**

Here's a quick example of how to use **react-native-easy-carousel** in your React Native project:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`javascriptCopy codeimport React from 'react';  import { Text, View, StyleSheet } from 'react-native';  import CarouselComponent from 'react-native-easy-carousel';  const App = () => {    const items = ['Item 1', 'Item 2', 'Item 3'];    const renderItem = (item, index) => (        {item}    );    return (`

              `items={items}          renderItem={renderItem}          autoplay          autoplayInterval={2000}          onIndexChanged={(index) => console.log('Current index:', index)}        />    );  };  const styles = StyleSheet.create({    container: {      flex: 1,    },    carouselItem: {      flex: 1,      justifyContent: 'center',      alignItems: 'center',      backgroundColor: '#ccc',    },  });  export default App;`

**API**

**CarouselComponent**

The main component that handles the horizontal scrolling, autoplay, and pagination.

**Props:**

- **items** (required): An array of items to be displayed in the carousel.
- **onIndexChanged** (optional): A callback function that is called when the index changes. Receives the new index as an argument.
- **autoplay** (optional): A boolean to enable or disable autoplay. Defaults to **false**.
- **autoplayInterval** (optional): The interval for autoplay in milliseconds. Defaults to **3000**.
- **renderItem** (required): A function that takes an item and its index and returns a React element to render.
- **containerStyle** (optional): Custom styles for the container.
- **itemStyle** (optional): Custom styles for each item.

**Example:**

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML

`javascriptCopy code  items={items}    renderItem={renderItem}    autoplay    autoplayInterval={2000}    onIndexChanged={(index) => console.log('Current index:', index)}    containerStyle={{ backgroundColor: 'white' }}    itemStyle={{ padding: 10 }}  />`

**Customization**

You can customize the carousel and its items by modifying the styles or adding additional props to the components.

**Styles:**

You can pass custom styles to the container and item components via the **containerStyle** and **itemStyle** props.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML

`javascriptCopy code  items={items}    renderItem={renderItem}    containerStyle={{ backgroundColor: 'white' }}    itemStyle={{ padding: 10 }}  />`

**Example**

Check out the example provided to see how to integrate the carousel into your app.

**Contributing**

Contributions are welcome! Please open an issue or submit a pull request to help improve the package.

**License**

This project is licensed under the ISC License.

**Repository**

For more details and to view the source code, visit the GitHub repository: [https://github.com/haewhydev/react-native-easy-carousel](https://github.com/haewhydev/react-native-easy-carousel)

This **README** content provides a comprehensive guide on how to use your **CarouselComponent**, including installation, usage, API details, customization options, and contribution guidelines, without using Markdown formatting.
