# Generate App Icons 📱

A simple and effective tool to generate icons for iOS and Android applications in different resolutions and styles.

## 🌟 Features

- 🖼️ Generates icons in different resolutions for Android: `mdpi`, `hdpi`, `xhdpi`, `xxhdpi`, `xxxhdpi`.
- 🖼️ Generates icons in various resolutions for iOS: as specified in `Contents.json`.
- 🎨 Android: Produces three distinct icon styles:
   - 🟥 Square (`ic_launcher_foreground.png`)
   - ⭕ Round (`ic_launcher_round.png`)
   - 🟩 Square with rounded edges (`ic_launcher.png`)

## 🔧 How to use

1️⃣ Clone this repo.

2️⃣ Install Dependencies

```sh
yarn add react-native-icon-generator
```

or

```sh
npm install react-native-icon-generator
```

3️⃣ Place the logo image (recommended 1024x1024) in the root folder and update the `inputImagePath` variable in the script with the correct path.

4️⃣ Run the command

```sh
npx react-native-icon-generator <path_to_logo.png> [--platform=ios|android]
```

5️⃣ Check the `output/icons` folder for the generated icons.

> Note: Replace `<path_to_logo.png>` with the path of your image. Use the `--platform` option to specify the desired platform (ios or android). If no platform is specified, both iOS and Android icons will be generated.

## ✏️ Customization

- Adjust the proportion of the icon in the "foreground" image by modifying the value `0.6` in `.resize(Math.round(config.square * 0.6))` for Android.
- Change the border radius for icons with rounded edges by modifying the `borderRadius` constant for Android.

## 📜 License

MIT