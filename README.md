# 🌈 Expo Blur Gradient on Scroll

![GitHub repo size](https://img.shields.io/github/repo-size/Masejg/expo-blur-gradient-on-scroll)
![GitHub stars](https://img.shields.io/github/stars/Masejg/expo-blur-gradient-on-scroll?style=social)
![GitHub forks](https://img.shields.io/github/forks/Masejg/expo-blur-gradient-on-scroll?style=social)

Welcome to the **Expo Blur Gradient on Scroll** repository! This project showcases an Expo Router app that features an animated gradient blur effect when scrolling. This README will guide you through the installation, usage, and contribution processes.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Contributing](#contributing)
6. [License](#license)
7. [Releases](#releases)

## Introduction

In modern app development, user experience is key. This project focuses on creating a visually appealing interface that captures user attention. The animated gradient blur effect enhances the scrolling experience, making it smooth and engaging. This repository aims to provide a simple way to implement this feature in your Expo apps.

## Features

- **Animated Gradient Blur**: Smooth transitions that enhance the visual appeal.
- **Responsive Design**: Works well on various screen sizes.
- **Easy Integration**: Simple setup process to get started quickly.
- **Well-Documented Code**: Clear comments and structure for easy understanding.

## Installation

To get started with this project, you need to have Node.js and Expo CLI installed on your machine. If you haven't installed them yet, follow these steps:

1. **Install Node.js**: Download and install from [nodejs.org](https://nodejs.org/).
2. **Install Expo CLI**: Run the following command in your terminal:

   ```bash
   npm install -g expo-cli
   ```

3. **Clone the repository**:

   ```bash
   git clone https://github.com/Masejg/expo-blur-gradient-on-scroll.git
   ```

4. **Navigate to the project directory**:

   ```bash
   cd expo-blur-gradient-on-scroll
   ```

5. **Install dependencies**:

   ```bash
   npm install
   ```

## Usage

After completing the installation, you can start the development server with:

```bash
expo start
```

This command will open a new browser window with the Expo developer tools. You can then scan the QR code with your Expo Go app to see the project in action on your mobile device.

### Customization

Feel free to customize the gradient colors and blur intensity in the main component file. The code is structured to allow easy modifications, enabling you to tailor the effect to fit your app's theme.

### Example

Here’s a quick example of how to implement the animated gradient blur in your app:

```javascript
import React from 'react';
import { View, Text, StyleSheet } from 'react-native';
import { LinearGradient } from 'expo-linear-gradient';
import { BlurView } from 'expo-blur';

const App = () => {
  return (
    <View style={styles.container}>
      <LinearGradient
        colors={['#ff7e5f', '#feb47b']}
        style={styles.gradient}
      >
        <BlurView intensity={50} style={styles.absolute}>
          <Text style={styles.text}>Welcome to Expo Blur Gradient!</Text>
        </BlurView>
      </LinearGradient>
    </View>
  );
};

const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
  gradient: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
  },
  absolute: {
    position: 'absolute',
    top: 0,
    left: 0,
    right: 0,
    bottom: 0,
    justifyContent: 'center',
    alignItems: 'center',
  },
  text: {
    color: '#fff',
    fontSize: 24,
  },
});

export default App;
```

## Contributing

We welcome contributions to improve this project. If you have suggestions, feel free to open an issue or submit a pull request. Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

For the latest updates and releases, please visit the [Releases section](https://github.com/Masejg/expo-blur-gradient-on-scroll/releases). Here, you can find downloadable files and instructions for executing them. Check it regularly for new features and improvements!

## Conclusion

Thank you for checking out the **Expo Blur Gradient on Scroll** project. We hope this repository serves as a useful resource for your app development needs. If you have any questions or feedback, feel free to reach out or open an issue.

Happy coding! 🌟