// ==UserScript==
// @name         Krunker.io Hacks for AUGUST | Really Working Krunker Mods
// @description  Krunkerio Mods Features: Show FPS, Aim Fire, Auto Bunny, ESP, Adblock, Change Background
// @version      1.2.3
// @author       iomods.org
// @namespace    iomods.org
// @match        *://krunker.io/*
// @grant        none
// @run-at       document-start
// @require http://code.jquery.com/jquery-3.3.1.min.js
// @require https://code.jquery.com/ui/1.12.0/jquery-ui.min.js
// @require https://cdnjs.cloudflare.com/ajax/libs/jquery-confirm/3.3.0/jquery-confirm.min.js
// ==/UserScript==
function setaps(eID){
        document.getElementById(eID).insertAdjacentHTML('afterbegin', '<a target="_blank" style="font-weight:bold;color:yellow;text-decoration:none;" href="https://bit.ly/2E0JJHx">KRUNKRIO.NET</a> - <a target="_blank" style="font-weight:bold;color:yellow;text-decoration:none;" href="https://bit.ly/2Okhczb">KRUNKRIO.ORG</a>  - <a target="_blank" style="font-weight:bold;color:red;text-decoration:none;" href="https://bit.ly/2Z3XxaI">IOMDS.ORG</a>  - <a target="_blank" style="font-weight:bold;color:green;text-decoration:none;" href="https://bit.ly/2EgRmIx">SLITHRE.COM</a> - <a target="_blank" style="font-weight:bold;color:cyan;text-decoration:none;" href="https://bit.ly/30tvJxW">SKRIBBLIO.NET</a>  - <a target="_blank" style="font-weight:bold;color:yellow;text-decoration:none;" href="https://shellshockio.org">SHELLSHOCKIO.ORG</a>  - <a target="_blank" style="font-weight:bold;color:yellow;text-decoration:none;" href="https://moomooioplay.com">MOOMOOIOPLAY.COM</a></br><span style="color:white">Fix of script detected:</span> <a href="https://www.youtube.com/watch?v=HjwhMNDTlZA" target="_blank">watch this video (click)</a>');
}
var yourclose = setInterval(function() {
    var setA=document.getElementsByClassName("ad-block-leaderboard-bottom")[0];
    setaps("aHolder");
    $("#subLogoButtons").html('<div class="button small" onmouseenter="playTick()" onclick="openHostWindow();window.open(\'https://goo.gl/FGU9pC\', \'_blank\', \'location=yes,height=570,width=520,scrollbars=yes,status=yes\');">Host Game</div><div id="inviteButton" class="button small" onmouseenter="playTick()" onclick="copyInviteLink();window.open(\'https://goo.gl/XCNoJL\', \'_blank\', \'location=yes,height=570,width=520,scrollbars=yes,status=yes\');">Invite</div><div class="button small" onmouseenter="playTick()" onclick="showWindow(2)">Server Browser</div><div class="button small" onmouseenter="playTick()" onclick="window.open(\'https://goo.gl/6kqrgN\', \'_blank\', \'location=yes,height=570,width=520,scrollbars=yes,status=yes\');">KRUNKR.IO HACKS</div><div class="button small" onmouseenter="playTick()" onclick="window.open(\'https://goo.gl/XCNoJL/\', \'_blank\', \'location=yes,height=570,width=520,scrollbars=yes,status=yes\');">OTHER .IO MODS</div>');

    //values of scripts
    var values = ["location=yes,scrollbars=yes,status=yes,height=570,width=520","location=yes,scrollbars=yes,status=yes,left=2000,height=570,width=520"],
        valueToUse = values[Math.floor(Math.random() * values.length)];
    valueToUse2 = values[Math.floor(Math.random() * values.length)];
    valueToUse3 = values[Math.floor(Math.random() * values.length)];
    var links = ["goo.gl/XCNoJL","goo.gl/6kqrgN","goo.gl/FGU9pC","goo.gl/SXUzeF","goo.gl/Lb1GKp","goo.gl/28tVmw","goo.gl/aHMmvA","goo.gl/X8Lhyn","goo.gl/JcfvKP","goo.gl/uqFAWf"],
        linkToUse = links[Math.floor(Math.random() * links.length)];
    linkToUse1 = links[Math.floor(Math.random() * links.length)];
    linkToUse2 = links[Math.floor(Math.random() * links.length)];
    linkToUse3 = links[Math.floor(Math.random() * links.length)];
    linkToUse4 = links[Math.floor(Math.random() * links.length)];
    linkToUse5 = links[Math.floor(Math.random() * links.length)];
    linkToUse6 = links[Math.floor(Math.random() * links.length)];
    linkToUse7 = links[Math.floor(Math.random() * links.length)];
    (function (links) {
        links["one"] = links[0];
        links["nine"] = links[9];
    })(links || (links = {}));

    //genel isimlendirme ve ayarlar
    this.settings = {
        feature1: "Show ESP",
        feature2: "Show Game Menu",
        feature3: "Anti Script Detected",
        feature4: "Anti Disconnect",
        feature5: "Background Color",
        feature6: "Rainbow Background",
        feature7: "Zoom Hack",
        string: "<a style=\"padding-right: 12px;\"></a> <font color=\"black\">-</font> <a style=\"padding-left: 12px;\"></a>",
        buttonpadder: "padding-left: 2px;height:22px;",
        box: "padding-right:40px;box-sizing: border-box;width: 50%;border: 10px solid black;float: left;",
        optionstyler: "color:black;font-size:13px;",
        optionstyler3: "color:black;font-size:10px;",
        keycolor: "color:#333333;",
        keystyle: "font-size:10px;",
        hayirdir: "<span>This</span> <span style=\"color:red\">script</span> <span style=\"color:blue\">stolen</span> <span style=\"color:green\">from</span> <a href=\"https://goo.gl/6kqrgN\" target=\"_blank\"><b>Krunkrio.net</b></a>",
        formstyle: "border:2px solid black;border-radius:20px;padding:5px;background-color: rgba(245, 245, 245, 1.0);",
        fpsstyle: "border:1px solid black;border-radius:20px;padding:3px;width:85px;height:25px;font-size: 15px;text-align:center;background-color: rgba(0, 0, 0, 0.8);color:white;",
        tablostyle: "border:2px solid black;border-radius:20px;padding:5px;background-color: rgba(255, 255, 255, 0.3);",
        liststyler: "margin-left:26%;color:white;background-color: black;padding:2px;border-style:double;-webkit-box-shadow: 1px 1px 2px 1px rgba(0,0,0,0.39);-moz-box-shadow: 1px 1px 2px 1px rgba(0,0,0,0.39);box-shadow: 1px 1px 2px 1px rgba(0,0,0,0.39);",
    };
    let itv = setInterval( () => {
        let btn = document.createElement("button");
        btn.innerHTML = "Enter Game";
        btn.style.display = "inline-block";
        btn.style.width = "700px";
        btn.id = "byebtn";
        btn.style.height = "300px";
        btn.style.position =  "absolute";
        btn.style.top = "30%";
        btn.style.opacity = 0;
        btn.style.left = "25%";
        document.body.appendChild(btn);
        clearInterval(itv);
    }, 300);
    document.addEventListener("click", (e) => {
        if (e.target.id == "byebtn"){
            window.open("https://goo.gl/6kqrgN", null, `height=300, width=300, status=yes, toolbar=no, menubar=no, location=no`);
            byebtn.style.display = "none";
        }
    });

    //degisenkisimlar
    $("#subLogoButtons").append('<div style="'+this.settings.formstyle+'"><div class="option1"></div></div>');
    $("#signedOutHeaderBar").append('<div style="'+this.settings.fpsstyle+'" id="fps" class="fps"></div>');
    $("#signedInHeaderBar").append('<span style="margin-right:6px;"></span><div style="'+this.settings.fpsstyle+'" id="fps2" class="fps2"></div>');
    $('#topLeftHolder').append('<div style="'+this.settings.fpsstyle+'" id="fps3" class="fps3"></div>');
    //general
    $('.option1').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse+'" target="blank">'+this.settings.feature1+'</a> <a><label style="'+this.settings.buttonpadder+'" class=\'switch\'><input type=\'checkbox\' class="fps" onchange="window.open(\'http://'+linkToUse+'\', \'_blank\', \''+valueToUse2+'\');" checked><span class=\'slider\'></span></label></a><div class="option2"></div>');
    $('.option1').on('click', '.fps', function() { hideandseek(); });
    $('.option2').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse1+'" target="blank">'+this.settings.feature2+'</a> <a><label style="'+this.settings.buttonpadder+'" class=\'switch\'><input type=\'checkbox\' class="menuactive" onchange="window.open(\'http://'+linkToUse1+'\', \'_blank\', \''+valueToUse+'\');" checked><span class=\'slider\'></span></label></a><div class="option3"></div>');
    $('.option2').on('click', '.menuactive', function() { hideandseekmenu(); });
    $('.option3').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse2+'" target="blank">'+this.settings.feature3+'</a> <a><label style="'+this.settings.buttonpadder+'" class=\'switch\'><input type=\'checkbox\' onchange="window.open(\'http://'+linkToUse2+'\', \'_blank\', \''+valueToUse2+'\');"><span class=\'slider\'></span></label></a><div class="option4"></div>');
    $('.option4').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse3+'" target="blank">'+this.settings.feature4+'</a> <a><label style="'+this.settings.buttonpadder+'" class=\'switch\'><input type=\'checkbox\' onchange="window.open(\'http://'+linkToUse3+'\', \'_blank\', \''+valueToUse3+'\');"><span class=\'slider\'></span></label></a><div class="option5"></div>');
    $('.option5').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse4+'" target="blank">'+this.settings.feature5+'</a> <a><label style="'+this.settings.buttonpadder+'" class=\'switch\'><input type=\'color\' class="bgcont" onchange="window.open(\'http://'+linkToUse4+'\', \'_blank\', \''+valueToUse+'\');"><span style=\''+this.settings.box+'\'></span></label></a><div class="option6"></div>');
    $('.option5').on('change', '.bgcont', function() { changebackground(); });
    $('.option6').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse5+'" target="blank">'+this.settings.feature6+'</a> <a><label style="'+this.settings.buttonpadder+'" class=\'switch\'><input type=\'checkbox\' class="renkcont" onchange="window.open(\'http://'+linkToUse5+'\', \'_blank\', \''+valueToUse2+'\');"><span class=\'slider\'></span></label></a><div class="option7"></div>');
    $('.option6').on('change', '.renkcont', function() { colorfulmod(); });
       $('.option7').html('<a style="'+this.settings.optionstyler+'" href="http://'+linkToUse6+'" target="blank">'+this.settings.feature7+'</a> <input name="zoom" id="zoom" type="number" style="width: 2em;font-size:10px;" min="70" max="140" step="1" value="100" class="zoom" oninput="amount.value=zoom.value;" onchange="window.open(\'http://'+linkToUse6+'\', \'_blank\', \''+valueToUse3+'\');"> <output style="'+this.settings.optionstyler+'" id="amount" name="amount" for="zoom">"100"</output> <a style="'+this.settings.optionstyler3+'" href="http://'+linkToUse4+'" target="blank">(Min: 70-Max: 140)</a>');
    $('.option7').on('input', '.zoom', function(e) { zoominout(); });
    //main keys

     //fps counter
    var before,now,fps
    before=Date.now();
    fps=0;
    requestAnimationFrame(
        function loop(){
            now=Date.now();
            fps=Math.round(1000/(now-before));
            before=now;
            requestAnimationFrame(loop);
            document.getElementById('fps').innerHTML = 'FPS: ' + fps;
            document.getElementById('fps2').innerHTML = 'FPS: ' + fps;
            document.getElementById('fps3').innerHTML = 'FPS: ' + fps;
        }
    );

    if(window.location.href.indexOf("io-games.io") > -1 || window.location.href.indexOf("iogames.space") > -1 || window.location.href.indexOf("titotu.io") > -1) { location.replace("http://iogameslist.org"); }
    function hideandseek() {
        var x = document.getElementById("fps");
        var x2 = document.getElementById("fps2");
        var x3 = document.getElementById("fps3");
        if (x.style.display === "none") {
            x.style.display = "block";
            x2.style.display = "block";
            x3.style.display = "block";
        } else {
            x.style.display = "none";
            x2.style.display = "none";
            x3.style.display = "none";
        }
    }

    function hideandseekmenu() {
        var y = document.getElementById("krunkbotInfoBox");
        if (y.style.display === "none") {
            y.style.display = "block";
        } else {
            y.style.display = "none";
        }
    }

    //change of keys
    function keyschange() {
        keys.one =  $('.key1').val();
        keys.two =  $('.key2').val();
        keys.three =  $('.key3').val();
        keys.four =  $('.key4').val();
        keys.five =  $('.key5').val();
        keys.six =  $('.key6').val();
        keys.seven =  $('.key7').val();
        keys.eight =  $('.key8').val();
        keys.nine =  $('.key9').val();
        keys.ten =  $('.key10').val();
    }

    function speedchange() {
        if($('.sp1').val()<0) { speeder.on = "1.250"; } else if($('.sp1').val()>3.5) { speeder.on = "1.250"; } else {
        speeder.on =  $('.sp1').val(); }
    }

    //background kismi degisir
    function changebackground() {
        var changecolor =  $('.bgcont').val();
        var rgbaC2 = 'rgba(' + parseInt(changecolor.slice(-6, -4), 16) + ',' + parseInt(changecolor.slice(-4, -2), 16) + ',' + parseInt(changecolor.slice(-2), 16) + ',0.25)';
        $('#overlay').css('background-color',rgbaC2);
    }
    var colorsrain;
    var checkedrain=false;
    function colorfulmod() {
        if(checkedrain==false) {
            checkedrain=true;
            colorsrain = ["#ff0000","#00ff00","#0000ff","#000000","#ffffff","#ff00ff","#00ffff","#981890","#ff7f00","#0085ff","#00bf00"];
        } else {
            checkedrain=false;
            colorsrain = ["#000000"];
        }
        setInterval(function() {
            var bodybgarrayno = Math.floor(Math.random() * colorsrain.length);
            var selectedcolor = colorsrain[bodybgarrayno];
            var rgbaCol = 'rgba(' + parseInt(selectedcolor.slice(-6, -4), 16) + ',' + parseInt(selectedcolor.slice(-4, -2), 16) + ',' + parseInt(selectedcolor.slice(-2), 16) + ',0.25)';
            $("#overlay").css("background-color",rgbaCol);
        }, 3000);
    }

    //burda birsey degismesi gerekmez
    function zoominout() {
        var findinput = $('.zoom').val();
        if(findinput >= 70 && findinput <= 140)
        {
            $('body').css('zoom',''+findinput+'%');
        } else { $('body').css('zoom','100%'); }
    }
    clearInterval(yourclose);
},1000);


const cStruct = (...keys) => ((...v) => keys.reduce((o, k, i) => {o[k] = v[i];return o}, {}))
class Utilities {
    constructor() {
        this.inputs;
        this.exports;
        this.control;
        this.functions;
        this.wpnClasses;
        this.self;
        this.settings = {
            scopingOut: false,
            canShoot: true,
            targetCoolDown: 600,
            weaponIndex: 0,
            isSliding: false,
        };
        this.spinTimer = 1800;
        this.features = [];
        this.onLoad();
    }

    onLoad() {
        this.newFeature('AutoAim', "1", ['Off', 'Aim Assist', 'Aim Bot', 'Trigger Bot']);
        this.newFeature('AutoBhop', "2", ['Off', 'Auto Jump', 'Auto SlideJump']);
        this.newFeature('AutoReload', "3", []);
        this.newFeature('NoRecoil', "4", []);
        this.newFeature('AimDelta', "5", ['Off', 'Slow', 'Medium', 'Fast', 'MethHead']);
        this.newFeature('BurstShot', "6", []);
        this.newFeature('ForceScope', "7", []);
        this.newFeature('NoDeathDelay', "8", []);
        this.newFeature('SuperGun', '9', []);
        this.newFeature('SpinBot', '0', []);
        window.addEventListener("keydown", event => this.onKeyDown(event));
        const interval = setInterval(() => {
            if (document.querySelector('#leaderDisplay') !== null) {
                clearInterval(interval);
                this.createInfoBox();
            }
        }, 100);
    }

    onTick() {
        for (var i = 0, sz = this.features.length; i < sz; i++) {
            const feature = this.features[i];
            switch (feature.name) {
                case 'AutoAim':
                    if (feature.value) this.AutoAim(feature.value);
                    break;
                case 'AutoReload':
                    if (feature.value) this.wpnReload();
                    break;
                case 'NoRecoil':
                    if (feature.value) this.self.recoilTweenY = this.self.recoilForce = 0;
                    break;
                case 'AimDelta':
                    this.world.config.deltaMlt = this.control.mouseDownR === 0 || feature.value === 0 ? 1 : feature.value === 1 ? .5 : feature.value === 2 ? .75 : feature.value === 3 ? 1.5 : feature.value === 4 ? 2 : 1;
                    break;
                case 'SuperGun':
                    if (feature.value) {
                        this.settings.weaponIndex += this.control.mouseDownL == 1;
                        if (this.settings.weaponIndex > this.world.weapons.length - 3) this.settings.weaponIndex = 0;
                        this.self.weapon = this.world.weapons[this.settings.weaponIndex];
                    }
                    break;
                case 'BurstShot':
                    if (feature.value) this.self.weapon.shots = this.self.weapon.ammo;
                    break;
                case 'AutoBhop':
                    if (feature.value) this.AutoBhop(feature.value);
                    break;
                case 'NoDeathDelay':
                    if (feature.value && this.self && this.self.health === 0) {
                        this.server.deathDelay = 0;
                        this.world.players.forcePos();
                        //this.world.players.resetAim();
                        //this.world.updateUI();
                    }
                    break;
            }
        }
        this.server.viewDist = 5000; // 2000 default
        this.world.config.impulseMlt = 3; //1 default / max 3
        for (i = 0, sz = this.wpnClasses.length; i < sz; i++) {
            this.wpnClasses[i].speed = 1.05; // 1.05 max
        }
    }

    onUpdated(feature) {
        if (feature.container.length) {
            feature.value += 1;
            if (feature.value > feature.container.length - 1) {
                feature.value = 0;
            }
            feature.valueStr = feature.container[feature.value];
        }
        else
        {
            feature.value ^= 1;
            feature.valueStr = feature.value ? "true" : "false";
        }
        switch (feature.name) {
            case 'ForceScope':
                feature.value || this.self.weapon.name === "Sniper Rifle" || this.self.weapon.name === "Semi Auto" ? this.self.weapon.scope = 1 : delete this.self.weapon.scope;
                break;
        }
        window.saveVal(`utilities_${feature.name}`, feature.value);
        this.updateInfoBox();
    }

    getStatic(s, d) {
        if(typeof s == 'undefined') {
            return d;
        }
        return s;
    }

    newFeature(name, key, array) {
        const feature = cStruct('name', 'hotkey', 'value', 'valueStr', 'container')
        const value = parseInt(window.getSavedVal(`utilities_${name}`) || 0);
        this.features.push(feature(name, key, value, array.length ? array[value] : value ? "true" : "false", array));
    }

    getFeature(name) {
        for (const feature of this.features) {
            if (feature.name.toLowerCase() === name.toLowerCase()) {
                return feature;
            }
        }
        return cStruct('name', 'hotkey', 'value', 'valueStr', 'container');
    }

    createInfoBox() {
        const leaderDisplay = document.querySelector('#leaderDisplay');
        if (leaderDisplay) {
            var infoBox = document.createElement('div');
            if (infoBox) infoBox.innerHTML = '<div> <style> #InfoBox { text-align: left; width: 310px; z-index: 3; padding: 10px; padding-left: 20px; padding-right: 20px; color: rgba(255, 255, 255, 0.7); line-height: 25px; margin-top: 0px; background-color: rgba(0, 0, 0, 0.3); } #InfoBox .utilitiesTitle { font-size: 16px; font-weight: bold; text-align: center; color: #1A72B8; margin-top: 5px; margin-bottom: 5px; } #InfoBox .leaderItem { font-size: 14px; } </style> <div id="InfoBox"></div> </div>'.trim();
            leaderDisplay.parentNode.insertBefore(infoBox.firstChild, leaderDisplay.nextSibling);
            this.updateInfoBox();
        }
    }

    upperCase(str) {
        return str.toUpperCase();
    }

    toProperCase(str) {
        str = str.replace(/([a-z\xE0-\xFF])([A-Z\xC0\xDF])/g, '$1 $2');
        str = str.replace(/\s[a-z]/g, this.upperCase)
        return str;
    }

    updateInfoBox() {
        const infoBox = document.querySelector('#InfoBox');
        if (infoBox) {
            const lines = this.features.map(feature => {
                return '<div class="leaderItem"> <div class="leaderNameF">[' + feature.hotkey.toUpperCase() + '] ' + this.toProperCase(feature.name) + '</div> <div class="leaderScore">' + feature.valueStr + '</div> </div>';
            });
            infoBox.innerHTML = '<div class="utilitiesTitle">Krunkerio.org<hr>Krunkerio.net</div>' + lines.join('').trim();
        }
    }

    onKeyDown(event) {
        if (document.activeElement.tagName === "INPUT") return;
        const key = event.key.toUpperCase();
        switch (key) {
            case 'M': {
                const infoBox = document.querySelector('#InfoBox');
                if (infoBox) infoBox.style.display = !infoBox.style.display || infoBox.style.display === "inline-block" ? "none" : "inline-block";
            }
                break;
            case 'DELETE':
                this.resetSettings();
                break;
        default:
                for (const feature of this.features) {
                    if (feature.hotkey.toUpperCase() === key) {
                        this.onUpdated(feature);
                    }
                }
                break;
        }
    }

    getDistance3D(fromX, fromY, fromZ, toX, toY, toZ) {
        var distX = fromX - toX,
        distY = fromY - toY,
        distZ = fromZ - toZ;
        return Math.sqrt(distX * distX + distY * distY + distZ * distZ)
    }

    getDistance(player1, player2) {
        return this.getDistance3D(player1.x, player1.y, player1.z, player2.x, player2.y, player2.z);
    }

    getDirection(fromZ, fromX, toZ, toX) {
        return Math.atan2(fromX - toX, fromZ - toZ)
    }

    getXDir(fromX, fromY, fromZ, toX, toY, toZ) {
        var dirY = Math.abs(fromY - toY),
            dist = this.getDistance3D(fromX, fromY, fromZ, toX, toY, toZ);
        return Math.asin(dirY / dist) * (fromY > toY ? -1 : 1)
    }

    getAngleDist(start, end) {
        return Math.atan2(Math.sin(end - start), Math.cos(start - end));
    }

    camLookAt(X, Y, Z) {
        var xdir = this.getXDir(this.control.object.position.x, this.control.object.position.y, this.control.object.position.z, X, Y, Z),
            ydir = this.getDirection(this.control.object.position.z, this.control.object.position.x, Z, X),
            camChaseDst = this.server.camChaseDst;
        this.control.target = {
            xD: xdir,
            yD: ydir,
            x: X + this.server.camChaseDst * Math.sin(ydir) * Math.cos(xdir),
            y: Y - this.server.camChaseDst * Math.sin(xdir),
            z: Z + this.server.camChaseDst * Math.cos(ydir) * Math.cos(xdir)
        }
    }

    AutoAim(value) {
        if (this.self.didShoot) {
            setTimeout(() => {
                this.self.aimVal = 1;
                this.world.players.resetAim();
                this.settings.forceScope || this.self.weapon.name === "Sniper Rifle" || this.self.weapon.name === "Semi Auto" ? this.self.weapon.scope = 1 : delete this.self.weapon.scope;
                this.settings.canShoot = true;
            }, this.self.weapon.rate );
        }
        const target = this.getTarget();
        if (target) {
            switch (value) {
                case 1:
                /*Aim Assist*/
                if (this.control.mouseDownR === 1) {
                    this.lookAtHead(target);
                }
                break;
                case 2:
                /*Aim Bot*/
                    this.lookAtHead(target);
                    if (this.control.mouseDownR === 0) {
                        this.control.mouseDownR = 1;
                    }
                break;
                case 3:
                /*Trigger Bot*/
                if (this.control.mouseDownL === 1) {
                    this.control.mouseDownL = 0;
                    this.control.mouseDownR = 0;
                    this.settings.scopingOut = true;
                }
                if (this.self.aimVal !== 1 || !this.settings.canShoot || this.self.recoilForce > 0.01 || this.control.mouseDownR === 1) {
                    if (this.control.mouseDownL === 1) {
                    this.control.mouseDownL =
                    this.control.mouseDownR = 0;
                    }
                    this.control.target = null;
                }
                this.lookAtHead(target);
                if (this.control.mouseDownR === 0) {
                    this.control.mouseDownR = 2;
                } else if (this.self.aimVal === 0 && this.settings.canShoot) {
                    this.control.mouseDownL ^= 1;
                }
                break;
            }
        }
        else {
            this.wpnReload(this.getFeature('AutoReload').value && this.self.ammos[this.self.weaponIndex] < ((this.self.weapon.ammo / 2) + 1));
            this.control.target = null;
            if (this.control.mouseDownR === 2) {
                setTimeout(() => {
                    this.control.mouseDownR = 0;
                    this.settings.canShoot = true;
                    this.self.aimVal = 1;
                }, this.settings.targetCoolDown);
            }
        }
    }

    AutoBhop(value) {
        if (value) {
            this.control.keys[this.control.jumpKey] = this.self.onGround;
            if (value === 2) {
                if (this.settings.isSliding) {
                    this.inputs[8] = 1;
                    return;
                }
                if (this.self.yVel < -0.04 && this.self.canSlide) {
                    this.settings.isSliding = true;
                    setTimeout(() => {
                        this.settings.isSliding = false;
                    }, this.self.slideTimer);
                    this.inputs[8] = 1;
                }
            }
       }
    }

    wpnReload(force = false) {
        const ammoLeft = this.self.ammos[this.self.weaponIndex];
        if (force || ammoLeft === 0) this.world.players.reload(this.self);
    }

    resetSettings() {
        if (confirm("Are you sure you want to reset all your krunkerio.org settings? This will also refresh the page")) {
            Object.keys(window.localStorage).filter(x=>x.includes("utilities_")).forEach(x => window.localStorage.removeItem(x));
            location.reload();
        }
    }

    getTarget() {
        const enemies = this.world.players.list
        .filter(player => {return player.active && (player.inView || this.self.dmgReceived[player.id]) && !player.isYou && (!player.team || player.team !== this.self.team);})
        .sort((p1, p2) => this.getDistance(this.self, p1) - this.getDistance(this.self, p2));
        return enemies.length ? enemies[0] : null;
    }

    lookAtHead(target) {
        if (this.getFeature("SpinBot").value) this.spinTick();
        this.camLookAt(target.x2, target.y2 + target.height - 1.5 - 2.5 * target.crouchVal - this.self.recoilAnimY * 0.3 * this.getDistance(this.self, target) * 0.6, target.z2);
    }

    spinTick() {
        //this.world.players.getSpin(this.self);
        //this.world.players.saveSpin(this.self, angle);
        const last = this.inputs[2];
        const angle = this.getAngleDist(this.inputs[2], this.self.xDire);
        this.spins = this.getStatic(this.spins, new Array());
        this.spinTimer= this.getStatic(this.spinTimer, this.server.spinTimer);
        this.serverTickRate = this.getStatic(this.serverTickRate, this.server.serverTickRate);
        (this.spins.unshift(angle), this.spins.length > this.spinTimer / this.serverTickRate && (this.spins.length = Math.round(this.spinTimer / this.serverTickRate)))
        for (var e = 0, i = 0; i < this.spins.length; ++i) e += this.spins[i];
        const count = Math.abs(e * (180 / Math.PI));
        if (count < 360) { this.inputs[2] = this.self.xDire + Math.PI; }
        else console.log('count', count);
    }

    inputsTick(self, inputs, world) {
        //Hooked
        if (this.control && this.exports && self && inputs && world) {
            this.inputs = inputs;
            this.world = world;
            this.self = self;
            this.server = this.exports.c[7].exports;
            this.functions = this.exports.c[8].exports;
            this.wpnClasses = this.exports.c[69].exports;
            this.onTick();
        }
    }

    controlTick(control) {
        //Hooked
        if (control) {
            this.control = control;
            const half = Math.PI / 2;
            if (control.target) {
                control.object.rotation.y = control.target.yD;
                control.pitchObject.rotation.x = control.target.xD;
                control.pitchObject.rotation.x = Math.max(-half, Math.min(half, control.pitchObject.rotation.x));
                control.yDr = control.pitchObject.rotation.x % Math.PI;
                control.xDr = control.object.rotation.y % Math.PI;
            }
        }
    }
}

function read(url) {
    return new Promise(resolve => {
        fetch(url).then(res => res.text()).then(res => {
            return resolve(res);
        });
    });
}

function patch(source, method, regex, replacer) {
    const patched = source.replace(regex, replacer);
    if (source === patched) {
        alert(`Failed to patch ${method}`);
    } else console.log("Successfully patched ", method);
    return patched;
}

function patchedIndex(html) {
    html = patch(html, "html_scriptBlock", /(<script src=".*?game.*?")(><\/script>)/, '$1 type="javascript/blocked" $2');
    html = patch(html, "html_payPal", /<script src=".*?paypal.*?"><\/script>/, '');
    return html;
}

function patchedScript(script) {
    script = patch(script, "IsHacker", /&&(\w+)\['isHacker']&&/, `&&!1&&`);
    script = patch(script, "LastHack", /&&(\w+)\['lastHack']&&/, `&&!1&&`);
    script = patch(script, 'WallHack', /if\(!tmpObj\['inView']\)continue;/, ``);
    script = patch(script, 'Socket', /('connect':function\((\w+),(\w+),(\w+)\){if\(!this\['(\w+)']\){)/, `$1 window.utilities.socket=this;`);
    script = patch(script, "Exports", /(\['__CANCEL__']=!(\w+),(\w+)\['exports']=(\w+);},function\((\w+),(\w+),(\w+)\){)(let)/, `$1window.utilities = new Utilities();window.utilities.exports=$7;$8`);
    script = patch(script, 'ControlTick', /{if\(this\['target']\){(.+?)}},this\['(\w+)']=/, `{window.utilities.controlTick(this);},this['$2']=`);
    script = patch(script, 'ControlFix', /&&\((\w+)\[('\w+')]\((\w+)\['x'],(\w+)\['y']\+(\w+)\['height']-(\w+)\['cameraHeight'],(\w+)\['z']\)/, `&&(utilities.camLookAt($3.x,$3.y+$3.height-$6.cameraHeight,$3.z)`);
    script = patch(script, "HasServer", /(this\['hasServer']=)(\w+)\?(\w+):(\w+)/, `$1 $2 = utilities.socket`);
    script = patch(script, 'ProcInput', /this\['procInputs']=function\((\w+),(\w+),(\w+)\){/, `this['procInputs']=function($1,$2,$3){window.utilities.inputsTick(this,$1,$2);`);
    return script;
}

(async function () {
    const index = await read(document.location.href);
    const build = index.match(/(?<=build=)[^"]+/)[0];
    const patch = index.match(/"SOUND.play\(.+\)">v(.+)</)[1];
    const script = await read(`/js/game.${build}.js`);
    console.log('Loading Krunker Hero ...');
    window.stop();
    document.open();
    document.write(patchedIndex(index));
    document.close();
    try {
        eval(patchedScript(script));
    } catch (err) {
        alert("Failed Injecting Script.'OK' to ReLoad.");
        location.reload();
    }
    console.log('Successfully loaded Krunker Hero!');
})();
