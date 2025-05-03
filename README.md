# 🫧 Enhanced D3 Bubble Chart Visualization

This project presents an interactive bubble chart visualization built using D3.js. It enhances upon the work of Jeffrey Morgan by adding several features for data exploration and interaction.

## ✨ Features

Based on the core implementation in `index.html` (framework) and `script.js` (functionality):

*   **Multiple Data Views:** Display bubble data grouped by:
    *   Combine (All bubbles together)
    *   Continent
    *   Country Centers
    *   Population (Bubble size representing population)
*   **Visual Toggles:** Switch between displaying `Colors` or `Flags` within the bubbles.
*   **Interactive Selection & Comparison:**
    *   Select individual or multiple bubbles by clicking.
    *   Display a dynamic bar chart comparing the populations of selected countries.
    *   Clear selected bubbles and the bar chart with a single action.
*   **Data Lookup:**
    *   Search for specific countries using a dedicated search box.
    *   Browse and select countries via a scrollable list.
*   **Fisheye Distortion:** Implemented using `fisheye.js`, this feature helps magnify smaller bubbles upon mouse hover, improving visibility of less prominent data points. It can be toggled on/off.

## 📁 File Structure & Data

*   `index.html`: Basic HTML structure for the visualization.
*   `script.js`: Core D3.js logic for bubble chart creation, interactions, transitions, bar chart, search, and fisheye integration.
*   `fisheye.js`: Implements the fisheye distortion effect.
*   `styles.css`: Contains CSS rules for positioning, colors, fonts, and other visual aspects of the components.
*   `flags.zip`: Archive containing flag images for each country. (Note: Needs to be unzipped, likely into a specific directory referenced by the code).
*   `continent-names.json`: Stores continent abbreviations or related data.
*   `countries.csv`: Contains country data including name, continent, total population, etc.

## ⚠️ Usage Notes & Limitations

Due to the nature of D3.js rendering and transitions:

*   **Visual Glitches:** If you experience sudden image movements or overlapping elements, try adjusting the zoom level using `Ctrl + Mouse Wheel` or enter full-screen mode by pressing `F11`.
*   **Bubble Confusion (Combine View):** If bubbles become tangled or confused, especially in the 'Combine' view after interactions, refreshing the page (`F5` or `Ctrl+R`) usually resolves the issue.

## 📸 Demonstration

Here are some demonstrations of the enhanced features:

*   **Float on Bubble Data Display Function:**
    ![1](https://github.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/blob/main/1-Float%20on%20Bubble%20Data%20Display%20Function.gif?raw=true)

*   **Multi-selected bubbles with bar graph comparison function and can be deleted with one click:**
    ![2](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/2-Multiple%20choice%20of%20bubbles%20and%20can%20be%20compared%20with%20the%20bar%20graph%20function%20and%20can%20be%20deleted%20with%20one%20click%20function.gif)

*   **Search Country Functions:**
    ![3](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/3-Search%20country%20function.gif)

*   **List scrolling country search function:**
    ![4](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/4-List%20scrolling%20query%20country%20function.gif)

*   **Opening and closing of the fisheye effect and the effect of using it:**
    ![5](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/5-Fisheye%20effect%20opening%20and%20closing%20and%20usage%20effects.gif)

## 🙏 Acknowledgements

This project builds upon and enhances the D3 Country Bubble Chart originally created by Jeffrey Morgan.
*   Original Repository: [https://github.com/jeffreymorganio/d3-country-bubble-chart](https://github.com/jeffreymorganio/d3-country-bubble-chart)

## 📄 许可证 (License)

本项目根据 **[MIT 许可证](https://opensource.org/licenses/MIT)** 条款进行许可。

这意味着您被授予了非常广泛的权利，可以自由地使用、复制、修改、合并、出版、分发、再许可 (sublicense) 和/或销售本软件的副本，并且可以允许获得软件副本的人也这样做，但须遵守以下条件：

*   上述版权声明和本许可声明必须包含在本软件的所有副本或主要部分中。

本软件按“原样”提供，不作任何形式的保证，无论是明示的还是默示的，包括但不限于对适销性、特定用途适用性和非侵权性的保证。在任何情况下，作者或版权持有人均不对任何索赔、损害或其他责任承担任何责任，无论是在合同诉讼、侵权行为还是其他方面，即使是因本软件或本软件的使用或其他处理方式而引起的或与之相关的。

有关完整的许可条款，请参阅项目根目录下的 [`LICENSE`](./LICENSE) 文件。
