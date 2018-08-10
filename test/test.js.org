// siple async test for HTTP 200 response code supertwst
'use strict';

var request = require("supertest"),
	app = require("/app").getApp;

describe('GET /', function(){
  it('expexts HTTP response 200', function(done){
	request(app)
	 .get('/')
	 .expect(200, done);
	});
});
