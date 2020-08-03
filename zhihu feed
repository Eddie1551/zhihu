let body = $response.body
body=JSON.parse(body)
delete body['ad_info']
body['data'].forEach((element, index)=> {
    if(element['author']['name']=="盐选推荐"||element['author']['name']=="盐选科普"||element['author']['name']=="故事档案局"||element['author']['name']=="知乎盐选会员"){ 
          body['data'].splice(index,1)  
     }
 })
body=JSON.stringify(body)
$done({body})
