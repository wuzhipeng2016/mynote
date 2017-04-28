JsonObject jsonObject = (new JsonParser()).parse(json).getAsJsonObject();
JsonObject json = (JsonObject)(new JsonParser()).parse(setting);
JsonObject json = (new JsonParser()).parse(setting).getAsJsonObject();
首先
map 转换为 String
		JsonObject jsonObject = new JsonObject();
		jsonObject.addProperty("name", "xxx");
		jsonObject.addProperty("value", "xxx");
		Gson gson = new Gson();
		String s = gson.toJson(jsonObject);
 
name 和 value 还有xxx可以从map中遍历而来
 
 
 
 
然后 string 转化为 map形式
		String s = "{\"name\":\"xiaolin\",\"value\":\"xxx\"}";
		JsonParser jp = new JsonParser();
		JsonObject jo = (JsonObject)jp.parse(s);
		System.out.println(jo.get("name").getAsString());


