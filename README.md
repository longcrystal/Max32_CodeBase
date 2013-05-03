<!DOCTYPE html>
<html>
    <head>
        <meta charset=ISO-8859-1>
    </head>
    <body>
        <div>
            <h1>Overview</h1>
            <p>This repository contains code projects with the Max32 microcontroller. The code projects are presented below.<p/>
            
            <dd>
                <h2><a href="./ADC_12bit/">ADC 12 bits code</a></h2>
                <p>This code project is about making the Max32 communicate via an SPI channel with a 12 bits ADC.</p>
                <a href="./ADC_12bit/doc">Documentation</a>
            </dd>
            <dd>
                <h2><a href="./lsm330a/">LSM330 accelerometer code</a></h2>
                <p>This code project is about making the Max32 communicate via an SPI channel with the LSM330 accelerometer.</p>
                <a href="./lsm330a/doc">Documentation</a>
            </dd>
            <dd>
                <h2><a href="./lsm330g/">LSM330 gyroscope code</a></h2>
                <p>This code project is about making the Max32 communicate via an SPI channel with the LSM330 gyroscope.</p>
                <a href="./lsm330g/doc">Documentation</a>
            </dd>
            <dd>
                <h2><a href="./L3G4200D/">L3G4200D gyroscope code</a></h2>
                <p>This code project is about making the Max32 communicate via an SPI channel with the L3G4200D gyroscope.</p>
                <a href="./L3G4200D/doc">Documentation</a>
            </dd>            
        </div>     
        <div>
            <h1>Prerequisites</h1>
            <ul>
                <li>
                    <p><a href="http://chipkit.org/wiki/?title=MPIDE_Installation">Download and install MPIDE</a></p>
                </li>
                <li>
                    <p><a href="http://www.digilentinc.com/Products/Detail.cfm?Prod=CHIPKIT-MAX32">Buy a Max32</a> (the code might work with other PIC chips)</p>
                </li>
                <li>
                    <p><a href="http://www.digikey.ca/product-detail/en/MCP3208-CI%2FP/MCP3208-CI%2FP-ND/305928?cur=USD">Buy a 12 bits ADC</a> (the code might work with other ADC chips)</p>
                </li>
                <li>
                    <p><a href="http://ca.mouser.com/ProductDetail/STMicroelectronics/LSM330DL/?qs=sGAEpiMZZMvhQj7WZhFIABvlHH1EqRb7AHxxrBGGw5U%3d">Buy an LSM330</a> (the codes might work with other gyro or accelerator chips)</p>
                </li>
                <li>
                    <p><a href="https://www.sparkfun.com/products/10612?">Buy a L3G4200D</a> (the code might work with other gyro chips)</p>
                </li>                
            </ul>
        </div>    
        <div>
            <h1>Program execution setup</h1>
            <ol>
                <li>Execute MPIDE on your pc</li>
                <li>Open a code project on your MPIDE (/File/Open.../)</li>
                <li>Choose the right board for the program execution (/Tools/Board/chipKIT MAX32)</li>
                <li>Choose the right port for the program execution on the board (/Tools/Serial Port/)</li>
                <li>Upload the code on your board (click    <img src="./img/upload.jpg/" style="padding:0 15px 0 15px;"></img>)</li>
                <li>Open the serial monitor and make sure you are listening on the right port at the right baud rate (click    <img src="./img/monitor.jpg/" style="padding:0 15px 0 15px;"></img>)</li>
                <li>You should read the output values on the monitor</li>
            </ol>
        </div>
        <div>
            <h1>Data interpretation</h1>
            <dd>
                <h2><a href="./ADC_12bit/">ADC 12 bits code</a></h2>
                <p>The ADC input value is calculated : AdcOutputValue/4096*5 = AdcInputValueInVolts</p>
                <p>For a 5V ADC input value, you should read 4096 on the monitor.</p>
                <p>For a 3.3V ADC input value, you should read a value around 2700 on the monitor.</p>
                <p>For a 0V ADC input value, you should read 0 on the monitor.</p>
                <a href="./ADC_12bit/doc">Documentation</a>
            </dd>
            <dd>
                <h2><a href="./lsm330a/">LSM330 accelerometer code</a></h2>
                <p>The LSM330 accelerometer output value is a linear acceleration measured in g</p>
                <a href="./lsm330a/doc">Documentation</a>
            </dd>
            <dd>
                <h2><a href="./lsm330g/">LSM330 gyroscope code</a></h2>
                <p>The LSM330 gyro output value is an angular rate measured in degrees per second (dps)</p>
                <a href="./lsm330g/doc">Documentation</a>
            </dd>
            <dd>
                <h2><a href="./L3G4200D/">L3G4200D gyroscope code</a></h2>
                <p>The L3G4200D output value is is an angular rate measured in degrees per second (dps)</p>
                <a href="./L3G4200D/doc">Documentation</a>
            </dd>
        </div>
        <div>
            <h1>Authors</h1>
            <ul>
                <li>Micha�l Fayad</li>
                <li>Rapha�l Guimond</li>
            </ul>
        </div>        
    </body>
</html>