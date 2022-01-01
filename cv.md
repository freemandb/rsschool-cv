# Dan Freeman

----

### FullStack Develope

----

### Contacts

**Cell Phone** +375(29)010203
**e-mail**     freemandb@mail.ru

----

### Brief Info:

>Draft text about my life, gained knowlege and ambitions

----

### Skills

+ HTML, CSS
+ JavaScript 
+ ActionScript (2/3)

+ VS code, Intellij Idea, WebStorm, Eclipse
+ Adobe Scout, Adobe Animate, Adobe Photoshop

----

### Code examples

>Simple node.js code

```
const onKeyPressHandler = async e => {
    let direction, up;
    if (["game-over", "win"].includes(gameStatus)) return;

    if (checkGameOver(data)) {
        setGameStatus("game-over");
        return;
    }

    switch (e.keyCode) {
        case 87: // W
            direction = "x";
            up = true;
            break;
        case 83: // S
            direction = "x";
            up = false;
            break;
        case 81: // Q
            direction = "z";
            up = true;
            break;
        case 68: // D
            direction = "z";
            up = false;
            break;
        case 69: // E
            direction = "y";
            up = false;
            break;
        case 65: // A
            direction = "y";
            up = true;
            break;
        default: return;
    }

    const dataAfterTurn = turn(data, direction, up, radius);

    if (!compareHexArray(data, dataAfterTurn)) {
        if (checkWin(dataAfterTurn)) {
            setGameStatus("win");
            return;
        }

        setGameStatus("loading");
        try {
            const fetchedData = await fetchNewData(dataAfterTurn, server, radius);
            setGameStatus("playing");
            if (checkGameOver(fetchedData)) {
                setGameStatus("game-over");
            }
            setData(fetchedData);
        } catch {
            setGameStatus("offline");
        }
    }
}
```
----

###Courses

+ HTML, CSS, JavaScript in RS School