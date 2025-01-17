# 浏览器简介


## 浏览器结构

浏览器一般包括DOM引擎、CSS解释器、脚本引擎、渲染引擎、协议支持、媒体流支持、第三方库、数据存储、用户界面等几个部分。

DOM引擎解析HTML、XML、SVG、MathML、XUL等内容。

CSS解释器解析CSS，为DOM中的各个元素计算样式信息。

渲染引擎根据元素与样式信息，计算大小、位置、布局，渲染解析后的内容。

脚本引擎包括JavaScript、VBScript、asm.js、WebAssembly等解释器，对脚本进行解释执行，并对DOM、CSS进行修改。

浏览器支持的协议通常包括HTTP、FTP、WebSocket、HTTP/2、QUIC、DNS、mDNS、WebRTC等。

浏览器支持的媒体流通常包括JPG、GIF、PNG、WebM、Ogg、AAC、MP3、MP4、FLAC等。

第三方库包括Skia, ffmpeg, ICU, NSS, OpenVR, libpng, sqlite等。

用户界面包括地址栏、前进/后退按钮、书签菜单等。

## 浏览器内核

浏览器内核比较主要的两部分是渲染引擎(Layout engineer或Rendering Engine)和JavaScript引擎。

渲染引擎负责取得网页的内容(HTML、XML、图像等等)、整理讯息(例如加入CSS等)，以及计算网页的显示方式，然后会输出至显示器或打印机。

浏览器的内核的不同对于网页的语法解释会有不同，所以渲染的效果也不相同。所有网页浏览器、电子邮件客户端以及其它需要编辑、显示网络内容的应用程序都需要内核。

JavaScript引擎则解析和执行JavaScript来实现网页的动态效果。最开始渲染引擎和JavaScript引擎并没有区分的很明确，后来JavaScript引擎越来越独立，内核就倾向于只指渲染引擎。
