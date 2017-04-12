## Self-Activating Fall Alert

### Description
The objective of this project is to create a wearable, user-friendly automatic fall detection and alert device. We are creating this device to give senior citizens peace of mind that help will arrive if they fall (even if they are unconscious).

### Parts
We used the following parts for our system:

- 9DOF Razor IMU
- Bluetooth Mate Gold
- 400 mAh Lithium-Ion Battery
- JST Connector (Male-to-Male)

### Fall-Detection Algorithm
In order to determine if a fall has occured, we needed to develop an algorithm to automatically detect falls based on IMU data. Based on research and testing, we determined that we can detect falls solely using acceleration data. By testing different scenarios such as sitting, standing, walking, lying down, etc. we were able to determine acceleration values that are present for normal every day actions. A fall, however, generates such high acceleration values that we can easily tell a fall apart from every day motions. We created an algorithm based on a threshold value, and if accelerations exceed this threshold, we can determine a fall has occured.



# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/FallAlert2017/alertwebsite.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
