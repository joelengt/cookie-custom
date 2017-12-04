# cookie-custom
custom cookie library


/* ECS5 */

``js
  Cookies.set('neko','my name');
  
  Cookies.set('usagi','my name', { expires: 5 });
  Cookies.get('neko');
  Cookies.delete('neko'):
``

/* with json */
var obj = {
  name: 'joel',
  lastname: 'gonzales'
}

/* set json */
var valueJSON = JSON.stringify(obj)
Cookies.set('human', valueJSON, { expires: 5, path: '/' })
Cookies.set('human_data', valueJSON)

/* get json */
var parseJSON = Cookies.get('human')
var valueParsed = JSON.parse(parseJSON)
