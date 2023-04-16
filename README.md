.disable-download img {
  pointer-events: none; }
@-webkit-keyframes rotate-forever {
  0% {
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -ms-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg); }
  100% {
    -webkit-transform: rotate(360deg);
    -moz-transform: rotate(360deg);
    -ms-transform: rotate(360deg);
    -o-transform: rotate(360deg);
    transform: rotate(360deg); } }

@-moz-keyframes rotate-forever {
  0% {
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -ms-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg); }
  100% {
    -webkit-transform: rotate(360deg);
    -moz-transform: rotate(360deg);
    -ms-transform: rotate(360deg);
    -o-transform: rotate(360deg);
    transform: rotate(360deg); } }

@keyframes rotate-forever {
  0% {
    -webkit-transform: rotate(0deg);
    -moz-transform: rotate(0deg);
    -ms-transform: rotate(0deg);
    -o-transform: rotate(0deg);
    transform: rotate(0deg); }
  100% {
    -webkit-transform: rotate(360deg);
    -moz-transform: rotate(360deg);
    -ms-transform: rotate(360deg);
    -o-transform: rotate(360deg);
    transform: rotate(360deg); } }

.lightbox-spinner {
  -webkit-animation-duration: 0.7s;
  -moz-animation-duration: 0.7s;
  animation-duration: 0.7s;
  -webkit-animation-iteration-count: infinite;
  -moz-animation-iteration-count: infinite;
  animation-iteration-count: infinite;
  -webkit-animation-name: rotate-forever;
  -moz-animation-name: rotate-forever;
  animation-name: rotate-forever;
  -webkit-animation-timing-function: linear;
  -moz-animation-timing-function: linear;
  animation-timing-function: linear;
  height: 30px;
  width: 30px;
  border: 4px solid #fff;
  border-right-color: transparent;
  border-radius: 50%;
  display: inline-block;
  opacity: 0.7; }
.link-transition a {
  transition: background 0.2s ease, color 0.2s ease; }
  .link-transition a svg {
    transition: fill 0.2s ease; }

.project-cover .details {
  transition: background 0.2s ease; }

.project-cover .title,
.project-cover .fields,
.project-cover .custom,
.project-cover .description,
.project-cover .date {
  transition: color 0.2s ease; }
html.lightbox-enabled,
html.lightbox-enabled body {
  overflow: hidden; }

html.lightbox-zoomed .lightbox-content {
  cursor: zoom-out;
  overflow: auto; }
  html.lightbox-zoomed .lightbox-content.zoomable-x {
    justify-content: flex-start; }
  html.lightbox-zoomed .lightbox-content.zoomable-y {
    align-items: baseline; }

html.lightbox-zoomed #lightbox-wrap img {
  max-width: inherit;
  max-height: inherit; }

html.lightbox-zoomed #lightbox-img-wrap .lightbox-extra {
  display: none; }

.lightbox-link,
.lightbox-content.zoomable {
  cursor: zoom-in; }

#lightbox-wrap .lightbox-contents {
  -moz-user-select: none;
  -webkit-user-select: none;
  -ms-user-select: none;
  user-select: none; }

.lightbox-content {
  align-items: center;
  display: flex;
  height: 100%;
  justify-content: center;
  opacity: 1;
  position: absolute;
  top: 0;
  transition: opacity .4s;
  width: 100vw; }

#lightbox-blocking {
  align-items: center;
  bottom: 0;
  display: flex;
  justify-content: center;
  left: 0;
  position: fixed;
  right: 0;
  top: 0;
  z-index: 1002; }
  #lightbox-blocking .lightbox-spinner {
    display: none; }

#lightbox-wrap {
  height: 100%;
  left: 0;
  position: fixed;
  top: 0;
  width: 100vw;
  z-index: 1001; }
  #lightbox-wrap .offscreen, #lightbox-wrap.offscreen {
    height: 0;
    overflow: hidden;
    visibility: hidden;
    -webkit-transform: translateX(-99999px);
    -ms-transform: translateX(-99999px);
    transform: translateX(-99999px);
    width: 0; }
  #lightbox-wrap.loading .lightbox-spinner {
    display: block; }
  #lightbox-wrap .hidden {
    opacity: 0; }
  #lightbox-wrap .lightbox-contents {
    display: inline-block;
    max-height: 100%;
    max-width: 100%; }
  #lightbox-wrap.single .next, #lightbox-wrap.single .next:hover,
  #lightbox-wrap.single .prev,
  #lightbox-wrap.single .prev:hover {
    display: none; }
  #lightbox-wrap.extras-hidden #lightbox-img-wrap .lightbox-extra {
    opacity: 0;
    transition: opacity 1s; }
  #lightbox-wrap img {
    max-height: 100vh;
    max-width: 100vw; }

#lightbox-inner-wrap {
  height: 100%;
  margin: auto;
  position: relative;
  z-index: 1003; }
  #lightbox-inner-wrap .control {
    cursor: pointer;
    position: absolute;
    z-index: 1003; }
  #lightbox-inner-wrap svg .lightbox-icon-bg {
    fill: #696969;
    opacity: .2; }
  #lightbox-inner-wrap svg:hover .lightbox-icon-bg {
    opacity: .4; }
  #lightbox-inner-wrap .next,
  #lightbox-inner-wrap .prev {
    height: 100vh;
    opacity: 0;
    top: 0;
    width: 30vw; }
    #lightbox-inner-wrap .next:hover,
    #lightbox-inner-wrap .prev:hover {
      opacity: 1; }
    #lightbox-inner-wrap .next.hidden,
    #lightbox-inner-wrap .prev.hidden {
      cursor: default; }
      #lightbox-inner-wrap .next.hidden svg,
      #lightbox-inner-wrap .prev.hidden svg {
        display: none; }
    #lightbox-inner-wrap .next svg,
    #lightbox-inner-wrap .prev svg {
      top: -webkit-calc(50% - 30px) ;
      top: calc(50% - 30px) ;
      position: absolute; }
      #lightbox-inner-wrap .next svg .lightbox-icon-arrow,
      #lightbox-inner-wrap .prev svg .lightbox-icon-arrow {
        fill: #FFFFFF; }
  #lightbox-inner-wrap .next {
    right: 0; }
    #lightbox-inner-wrap .next svg {
      right: 20px; }
  #lightbox-inner-wrap .prev {
    left: 0; }
    #lightbox-inner-wrap .prev svg {
      left: 20px; }
  #lightbox-inner-wrap .close {
    position: fixed;
    height: 40px;
    right: 20px;
    top: 20px;
    width: 40px; }
    #lightbox-inner-wrap .close:hover {
      cursor: pointer; }
    #lightbox-inner-wrap .close .lightbox-icon-bg {
      fill: #fff; }

@media (max-width: 1024px) {
  #lightbox-inner-wrap .close {
    right: 0;
    top: 0; }
    #lightbox-inner-wrap .close circle {
      display: none; }
  #lightbox-inner-wrap .next:hover,
  #lightbox-inner-wrap .prev:hover {
    opacity: 0; } }

@media (min-width: 1024px) {
  .lightbox-link.hover-icon-enabled {
    position: relative; }
    .lightbox-link.hover-icon-enabled:hover::after {
      background: rgba(105, 105, 105, 0.2) url(data:image/svg+xml;base64,PHN2ZyBzdHlsZT0iZmlsbDogd2hpdGUiIHZpZXdCb3g9IjAgMCAyMSAyMSIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4KICA8cGF0aCBkPSJNLTEuMjUyMjIyNTEsMTUuNjAzNDE5NyBDLTEuMzUyNTE5MjcsMTUuNjkzNjg2OCAtMS40MjUyMzMzMywxNS43OTg5OTY4IC0xLjQ3MDM2Njg3LDE1LjkxOTM1MjkgQy0xLjUxNTUwMDQxLDE2LjAzOTcwOSAtMS41MzgwNjY4NCwxNi4xNjAwNjMzIC0xLjUzODA2Njg0LDE2LjI4MDQxOTQgQy0xLjUzODA2Njg0LDE2LjQwMDc3NTUgLTEuNTE1NTAwNDEsMTYuNTIxMTI5OCAtMS40NzAzNjY4NywxNi42NDE0ODU5IEMtMS40MjUyMzMzMywxNi43NjE4NDIgLTEuMzUyNTE5MjcsMTYuODY3MTUyIC0xLjI1MjIyMjUxLDE2Ljk1NzQxOTEgTDMuNTYxOTk3NzEsMjEuNzcxNjM5MyBDMy43NTI1NjE1NSwyMS45NjIyMDMyIDMuOTgwNzMzMjQsMjIuMDU3NDgzNyA0LjI0NjUxOTY1LDIyLjA1NzQ4MzcgQzQuNTEyMzA2MDUsMjIuMDU3NDgzNyA0LjczNTQ2Mjk5LDIxLjk2MjIwMzIgNC45MTU5OTcxNSwyMS43NzE2MzkzIEM1LjEwNjU2MDk4LDIxLjU4MTA3NTUgNS4yMDE4NDE0NywyMS4zNTU0MTEyIDUuMjAxODQxNDcsMjEuMDk0NjM5NiBDNS4yMDE4NDE0NywyMC44MzM4NjggNS4xMDY1NjA5OCwyMC42MDgyMDM3IDQuOTE1OTk3MTUsMjAuNDE3NjM5OSBMMS43NTY2NjUxMywxNy4yNDMyNjM0IEwxMC4wMTYwNjE3LDE3LjI0MzI2MzQgQzEwLjI4Njg2MjksMTcuMjQzMjYzNCAxMC41MTUwMzQ2LDE3LjE1MDQ5MDMgMTAuNzAwNTgzNiwxNi45NjQ5NDEzIEMxMC44ODYxMzI2LDE2Ljc3OTM5MjMgMTAuOTc4OTA1NywxNi41NTEyMjA2IDEwLjk3ODkwNTcsMTYuMjgwNDE5NCBDMTAuOTc4OTA1NywxNi4wMDk2MTgyIDEwLjg4NjEzMjYsMTUuNzgxNDQ2NSAxMC43MDA1ODM2LDE1LjU5NTg5NzUgQzEwLjUxNTAzNDYsMTUuNDEwMzQ4NSAxMC4yODY4NjI5LDE1LjMxNzU3NTMgMTAuMDE2MDYxNywxNS4zMTc1NzUzIEwxLjc1NjY2NTEzLDE1LjMxNzU3NTMgTDQuOTE1OTk3MTUsMTIuMTQzMTk4OSBDNS4xMDY1NjA5OCwxMS45NTI2MzUxIDUuMjAxODQxNDcsMTEuNzI2OTcwNyA1LjIwMTg0MTQ3LDExLjQ2NjE5OTIgQzUuMjAxODQxNDcsMTEuMjA1NDI3NiA1LjEwNjU2MDk4LDEwLjk3OTc2MzMgNC45MTU5OTcxNSwxMC43ODkxOTk1IEM0LjczNTQ2Mjk5LDEwLjU5ODYzNTYgNC41MTIzMDYwNSwxMC41MDMzNTUxIDQuMjQ2NTE5NjUsMTAuNTAzMzU1MSBDMy45ODA3MzMyNCwxMC41MDMzNTUxIDMuNzUyNTYxNTUsMTAuNTk4NjM1NiAzLjU2MTk5NzcxLDEwLjc4OTE5OTUgTC0xLjI1MjIyMjUxLDE1LjYwMzQxOTcgWiIgaWQ9IngiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQuNzIwNDE5LCAxNi4yODA0MTkpIHJvdGF0ZSgtNDUuMDAwMDAwKSB0cmFuc2xhdGUoLTQuNzIwNDE5LCAtMTYuMjgwNDE5KSAiPjwvcGF0aD4KICA8cGF0aCBkPSJNMTAuMzA3Nzc3NCw0LjA0MzQxOTczIEMxMC4yMDc0ODA3LDQuMTMzNjg2ODEgMTAuMTM0NzY2Niw0LjIzODk5NjgzIDEwLjA4OTYzMzEsNC4zNTkzNTI5MyBDMTAuMDQ0NDk5NSw0LjQ3OTcwOTA0IDEwLjAyMTkzMzEsNC42MDAwNjMzNCAxMC4wMjE5MzMxLDQuNzIwNDE5NDUgQzEwLjAyMTkzMzEsNC44NDA3NzU1NiAxMC4wNDQ0OTk1LDQuOTYxMTI5ODYgMTAuMDg5NjMzMSw1LjA4MTQ4NTk3IEMxMC4xMzQ3NjY2LDUuMjAxODQyMDcgMTAuMjA3NDgwNyw1LjMwNzE1MjA5IDEwLjMwNzc3NzQsNS4zOTc0MTkxNyBMMTUuMTIxOTk3NywxMC4yMTE2Mzk0IEMxNS4zMTI1NjE1LDEwLjQwMjIwMzIgMTUuNTQwNzMzMiwxMC40OTc0ODM3IDE1LjgwNjUxOTYsMTAuNDk3NDgzNyBDMTYuMDcyMzA2LDEwLjQ5NzQ4MzcgMTYuMjk1NDYyOSwxMC40MDIyMDMyIDE2LjQ3NTk5NzEsMTAuMjExNjM5NCBDMTYuNjY2NTYwOSwxMC4wMjEwNzU2IDE2Ljc2MTg0MTQsOS43OTU0MTEyNCAxNi43NjE4NDE0LDkuNTM0NjM5NjcgQzE2Ljc2MTg0MTQsOS4yNzM4NjgxMSAxNi42NjY1NjA5LDkuMDQ4MjAzNzkgMTYuNDc1OTk3MSw4Ljg1NzYzOTk1IEwxMy4zMTY2NjUxLDUuNjgzMjYzNDkgTDIxLjU3NjA2MTYsNS42ODMyNjM0OSBDMjEuODQ2ODYyOSw1LjY4MzI2MzQ5IDIyLjA3NTAzNDYsNS41OTA0OTAzOSAyMi4yNjA1ODM2LDUuNDA0OTQxMzkgQzIyLjQ0NjEzMjYsNS4yMTkzOTIzOSAyMi41Mzg5MDU3LDQuOTkxMjIwNjkgMjIuNTM4OTA1Nyw0LjcyMDQxOTQ1IEMyMi41Mzg5MDU3LDQuNDQ5NjE4MjEgMjIuNDQ2MTMyNiw0LjIyMTQ0NjUxIDIyLjI2MDU4MzYsNC4wMzU4OTc1MSBDMjIuMDc1MDM0NiwzLjg1MDM0ODUxIDIxLjg0Njg2MjksMy43NTc1NzU0MSAyMS41NzYwNjE2LDMuNzU3NTc1NDEgTDEzLjMxNjY2NTEsMy43NTc1NzU0MSBMMTYuNDc1OTk3MSwwLjU4MzE5ODk0NyBDMTYuNjY2NTYwOSwwLjM5MjYzNTExMSAxNi43NjE4NDE0LDAuMTY2OTcwNzk0IDE2Ljc2MTg0MTQsLTAuMDkzODAwNzcxNSBDMTYuNzYxODQxNCwtMC4zNTQ1NzIzMzcgMTYuNjY2NTYwOSwtMC41ODAyMzY2NTQgMTYuNDc1OTk3MSwtMC43NzA4MDA0OSBDMTYuMjk1NDYyOSwtMC45NjEzNjQzMjcgMTYuMDcyMzA2LC0xLjA1NjY0NDgyIDE1LjgwNjUxOTYsLTEuMDU2NjQ0ODIgQzE1LjU0MDczMzIsLTEuMDU2NjQ0ODIgMTUuMzEyNTYxNSwtMC45NjEzNjQzMjcgMTUuMTIxOTk3NywtMC43NzA4MDA0OSBMMTAuMzA3Nzc3NCw0LjA0MzQxOTczIFoiIGlkPSJ4IiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNi4yODA0MTksIDQuNzIwNDE5KSByb3RhdGUoLTIyNS4wMDAwMDApIHRyYW5zbGF0ZSgtMTYuMjgwNDE5LCAtNC43MjA0MTkpICI+PC9wYXRoPgo8L3N2Zz4K) no-repeat center;
      background-size: 16px;
      border-radius: 50%;
      content: '';
      display: block;
      height: 36px;
      position: absolute;
      right: 10px;
      top: 10px;
      width: 36px;
      z-index: 1000; } }

@media all and (-ms-high-contrast: none) {
  .lightbox-link,
  .lightbox-content.zoomable {
    cursor: pointer; } }
@-webkit-keyframes fade-in {
  from {
    opacity: 0; }
  to {
    opacity: 1; } }

@-moz-keyframes fade-in {
  from {
    opacity: 0; }
  to {
    opacity: 1; } }

@keyframes fade-in {
  from {
    opacity: 0; }
  to {
    opacity: 1; } }

@-webkit-keyframes fade-out {
  from {
    opacity: 1; }
  to {
    opacity: 0; } }

@-moz-keyframes fade-out {
  from {
    opacity: 1; }
  to {
    opacity: 0; } }

@keyframes fade-out {
  from {
    opacity: 1; }
  to {
    opacity: 0; } }

.transition-enabled {
  opacity: 0; }

.transition-in {
  -webkit-animation: fade-in ease-in;
  animation: fade-in ease-in;
  -webkit-animation-duration: 0.25s;
  animation-duration: 0.25s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards; }

.transition-out {
  opacity: 1;
  -webkit-animation: fade-out ease-out;
  animation: fade-out ease-out;
  -webkit-animation-duration: 0.25s;
  animation-duration: 0.25s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards; }
