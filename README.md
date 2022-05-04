# RestAssured

Sample Rest Assured Code

RestAssured.baseUri = "endpoint";
RestAssured.authentication = RestAssured.basic("","");


Response response = RestAssured.
                    given()
                        .ContentType(ContentType.json)
                        .accept(json)
                        .queryParam()
                        .log()
                        .all()
                    .when()
                        .get()
                    .then()
                        .log()
                        .all()
                        .assertThat()
                        .StatusCode(200)
                     
