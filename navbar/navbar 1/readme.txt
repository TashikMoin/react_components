link -> https://www.npmjs.com/package/@acto/react-navbar
npm install @acto/react-navbar




import * as React from 'react'
import Navbar from '@acto/react-navbar'
 
const navTheme = {
  mainColor: '#52b788',
  menuBgColor: '#edf7f3'
}
 
const navBrand = <a href="">Base Corp.</a>
 
const leftLinks = (
  <>
    <a href="">Our Plans</a>
    <a href="">How It Works</a>
    <a href="">Our Menus</a>
  </>
)
 
const rightLinks = (
  <>
    <a href="">Get Started</a>
    <a href="">Sign In</a>
  </>
)
 
const Example = () => {
  return (
    <div className="app">
      <Navbar
        className="navbar" // style .navbar in your css
        menuClassName="navbar--menu" // style .navbar--menu in your css
        brand={navBrand}
        theme={navTheme}
        leftLinks={leftLinks}
        rightLinks={rightLinks}
      />
    </div>
  )
}


