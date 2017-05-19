
5ef93b7d9500f0ada6f78032972605ea




ÃÜÔ¿
CjqMEknZKv0cRyAhzn6cJo5Arq1YLjL3XBD6fvuYFUG

bxw2359430729.my3w.com

ew-2q5e7l8ki.aliapp.com

$host = "http://jisutqybmf.market.alicloudapi.com";
    $path = "/weather/query";
    $method = "GET";
    $appcode = "Äã×Ô¼ºµÄAppCode";
    $headers = array();
    array_push($headers, "Authorization:APPCODE " . $appcode);
    $querys = "city=%E5%AE%89%E9%A1%BA&citycode=citycode&cityid=cityid&ip=ip&location=location";
    $bodys = "";
    $url = $host . $path . "?" . $querys;

    $curl = curl_init();
    curl_setopt($curl, CURLOPT_CUSTOMREQUEST, $method);
    curl_setopt($curl, CURLOPT_URL, $url);
    curl_setopt($curl, CURLOPT_HTTPHEADER, $headers);
    curl_setopt($curl, CURLOPT_FAILONERROR, false);
    curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);
    curl_setopt($curl, CURLOPT_HEADER, true);
    if (1 == strpos("$".$host, "https://"))
    {
        curl_setopt($curl, CURLOPT_SSL_VERIFYPEER, false);
        curl_setopt($curl, CURLOPT_SSL_VERIFYHOST, false);
    }
    var_dump(curl_exec($curl));