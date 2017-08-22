1、ajax的步骤

    1) let xhr = new XMLHttpRequest()
    2) xhr.open(method, url, async)
    3) xhr.setRequestHeader('Content-Type', contentType)
    4) xhr.onreadystatechange = handle
    5) xhr.send(data)
    
 注意：第三步setRequestHeader必须在第二步之后，
         因为只有open状态的xhr才可以调用setRequestHeader