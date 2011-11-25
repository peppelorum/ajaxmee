Ajaxmee is a small library to help ease the burden with ajax requests for devices like Nokia N9/N950 etc. It's a very simple library that uses nothing but XMLHttpRequest. The library takes five arguments, method type, url, data, success callback and error callback. Th data variable should be a dictionary and is flattened before posting.


Examples
--------

GET


     var data  = { 'key': key, 'from': from, 'to': to, 'coordSys': 'RT90', 'apiVersion': 2.1 }
     ajaxmee('GET', url, data,
        function(data) {
            console.log('ok', data)
        },
        function(status, statusText) {
            console.log('error', status, statusText)
        })


POST


    var data = { 'key': key, 'from': from, 'to': to, 'coordSys': 'RT90', 'apiVersion': 2.1 }
    ajaxmee('POST', url, data,
        function(data) {
            console.log('ok', data)
        },
        function(status, statusText) {
            console.log('error', status, statusText)
        })




