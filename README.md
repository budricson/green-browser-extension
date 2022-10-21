<h1 align="left">Building a Carbon Usage Browser Extension</h1>

Using tmrow's C02 Signal API to track electricity usage, I built a browser extension so that you can have a reminder right in your browser about how heavy your region's electricity usage is. Using this extension ad hoc will help you to make judgement calls on your activities based on this information.

<h2>Getting Started</h2>
You will need to have NPM installed. Download a copy of this code to a folder on your computer.

Install all the required packages:

```
npm install
```

Build the extension from webpack

```
npm run build
```

To install on Edge, use the 'three dot' menu on the top right corner of the browser to find the Extensions panel. From there, select 'Load Unpacked' to load a new extension. Open the 'dist' folder at the prompt and the extension will load. To use it, you will need an API key for CO2 Signal's API ([get one here via email](https://www.co2signal.com/) - enter your email in the box on this page) and the [code for your region](http://api.electricitymap.org/v3/zones) corresponding to the [Electricity Map](https://www.electricitymap.org/map) (in London, for example, I use 'GB').

Once the API key and region is input into the extension interface, the colored dot in the browser extension bar should change to reflect your region's energy usage and give you a pointer on what energy-heavy activities would be appropriate for you to perform. The concept behind this 'dot' system was given to me by the [Energy Lollipop extension](https://energylollipop.com/) for California emissions.

<h2>Credits</h2>

Building browser extensions is a fun and interesting way to think about the performance of your apps while building a different type of web asset. I followed this <a href="https://github.com/microsoft/Web-Dev-For-Beginners/tree/main/5-browser-extension">module</a> on how browsers work and how to deploy a browser extension, how to build a form, call an API, and use local storage, and how to gauge the performance of your website and improve it.
