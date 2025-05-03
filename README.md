# 🫧 Enhanced D3 Bubble Chart Visualization

This project presents an interactive D3.js bubble chart visualization. It builds upon the original work by Jeffrey Morgan, adding several features for enhanced data exploration and user interaction.

## ✨ Features

*   **Multiple Data Views:** Display bubble data grouped by:
    *   `Combine`: All bubbles displayed together.
    *   `Continent`: Bubbles grouped by their respective continents.
    *   `Country Centers`: Bubbles positioned based on geographical centers (conceptual).
    *   `Population`: Bubble size directly represents country population.
*   **Visual Toggles:** Switch the visual representation within bubbles between:
    *   `Colors`: Bubbles filled with distinct colors (e.g., per continent).
    *   `Flags`: Bubbles display the corresponding country's flag.
*   **Interactive Selection & Comparison:**
    *   Select individual or multiple bubbles by clicking.
    *   View a dynamically generated bar chart comparing the populations of the selected countries.
    *   Clear all selected bubbles and reset the comparison bar chart with a single "Clear Selections" action.
*   **Data Lookup & Browsing:**
    *   Search for specific countries using the dedicated search input box.
    *   Browse and select countries directly from a scrollable list panel.
*   **Toggleable Fisheye Distortion:**
    *   Leverages `fisheye.js` to provide a magnification effect on hover.
    *   Helps in exploring smaller, densely packed bubbles.
    *   This effect can be easily toggled on or off via a checkbox.

## 📁 File Structure

```
.
├── index.html          # Main HTML structure for the visualization
├── script.js           # Core D3.js logic (chart creation, interactions, transitions, bar chart, search, fisheye)
├── fisheye.js          # Implements the fisheye distortion effect
├── styles.css          # CSS rules for styling and layout
├── flags/              # Directory containing country flag images (Requires unzipping flags.zip here)
├── flags.zip           # Archive of country flag images
├── continent-names.json # Data mapping continent abbreviations or names
├── countries.csv       # Primary dataset (country name, continent, population, etc.)
└── LICENSE             # Project license file (MIT)
```

## 🚀 Setup & Usage

1.  **Clone the Repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
2.  **Unzip Flags:** Extract the contents of `flags.zip` into a directory named `flags` within the project's root directory. The structure should look like `flags/ad.png`, `flags/ae.png`, etc.
3.  **Run Locally:**
    *   **Simple Method:** Open the `index.html` file directly in your web browser. *Note: Some browsers have security restrictions regarding local file access (`file:///...`) which might interfere with loading data files (`.csv`, `.json`).*
    *   **Recommended Method:** Use a simple local web server. If you have Python installed, you can run:
        ```bash
        # Python 3.x
        python -m http.server
        # Python 2.x
        python -m SimpleHTTPServer
        ```
        Then, navigate to `http://localhost:8000` (or the port indicated) in your browser.

4.  **Interact:**
    *   Use the top control buttons to switch between data views and visual styles (`Colors`/`Flags`).
    *   Click on bubbles to select them for comparison.
    *   Use the search box or the country list to find specific countries.
    *   Use the "Clear Selections" button to reset the comparison chart and selections.
    *   Toggle the "Fisheye" checkbox to enable/disable the magnification effect on hover.

## ⚠️ Troubleshooting & Notes

*   **Visual Glitches:** Due to the nature of D3.js transitions, you might occasionally observe unexpected element movements or overlaps. Try adjusting your browser's zoom level (`Ctrl` + Mouse Wheel) or entering/exiting fullscreen mode (`F11`).
*   **Tangled Bubbles ('Combine' View):** If bubbles become heavily overlapped or visually "stuck" after many interactions, especially in the 'Combine' view, refreshing the web page (`F5` or `Ctrl+R`) typically resolves the layout issues.
*   **Data Loading:** Ensure the `countries.csv` and `continent-names.json` files are accessible relative to `index.html` (they should be in the same directory or the paths in `script.js` adjusted accordingly). The flags must be correctly placed in the `flags/` directory.

## 📸 Demonstration GIFs

*   **Tooltip Data Display on Hover:**
    ![1](https://github.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/blob/main/1-Float%20on%20Bubble%20Data%20Display%20Function.gif?raw=true)

*   **Multi-Select Bubbles & Bar Graph Comparison (with Clear):**
    ![2](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/2-Multiple%20choice%20of%20bubbles%20and%20can%20be%20compared%20with%20the%20bar%20graph%20function%20and%20can%20be%20deleted%20with%20one%20click%20function.gif)

*   **Country Search Functionality:**
    ![3](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/3-Search%20country%20function.gif)

*   **Scrollable Country List Selection:**
    ![4](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/4-List%20scrolling%20query%20country%20function.gif)

*   **Fisheye Effect Toggle & Usage:**
    ![5](https://raw.githubusercontent.com/WEllin06/A-Bubble-Chart-With-Tremendous-Function/main/5-Fisheye%20effect%20opening%20and%20closing%20and%20usage%20effects.gif)

## 🙏 Acknowledgements

This project significantly enhances and builds upon the D3 Country Bubble Chart originally created by Jeffrey Morgan.
*   Original Repository: [https://github.com/jeffreymorganio/d3-country-bubble-chart](https://github.com/jeffreymorganio/d3-country-bubble-chart)

## 📄 License

This project is licensed under the terms of the **[MIT License](https://opensource.org/licenses/MIT)**.

This means you are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, subject to the following conditions:

*   The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

The software is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.

For the full license text, please see the [`LICENSE`](./LICENSE) file in the project's root directory.
