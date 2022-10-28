# IssueTrackerSystem
{
	"info": {
		"_postman_id": "879aed5b-73d2-4391-8a52-94d59dd625ae",
		"name": "issue-tracker-api",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "3665338"
	},
	"item": [
		{
			"name": "addUser",
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"firstName\": \"chetan\",\r\n    \"lastName\": \"chetan\",\r\n    \"email\": \"chetan@gmail.com\",\r\n    \"active\": \"true\",\r\n    \"userName\": \"chetan\",\r\n    \"password\": \"chetan\",\r\n    \"roleId\": 2,\r\n    \"positionId\": 2\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/users/addUser",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"users",
						"addUser"
					]
				}
			},
			"response": []
		},
		{
			"name": "updateUser",
			"request": {
				"method": "PUT",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"firstName\": \"Roman\",\r\n    \"lastName\": \"Reigns\",\r\n    \"email\": \"roman@gmail.com\",\r\n    \"active\": \"true\",\r\n    \"userName\": \"roman\",\r\n    \"password\": \"roman\",\r\n    \"roleId\": 2,\r\n    \"positionId\": 2\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/users/updateUser/3",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"users",
						"updateUser",
						"3"
					]
				}
			},
			"response": []
		},
		{
			"name": "deleteUser",
			"request": {
				"method": "DELETE",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/users/deleteUser/3",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"users",
						"deleteUser",
						"3"
					]
				}
			},
			"response": []
		},
		{
			"name": "getAllUsers",
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"method": "GET",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"firstName\": \"chetan\",\r\n    \"lastName\": \"chetan\",\r\n    \"email\": \"chetan@gmail.com\",\r\n    \"active\": \"true\",\r\n    \"userName\": \"chetan\",\r\n    \"password\": \"chetan\",\r\n    \"roleId\": 2,\r\n    \"positionId\": 2\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/users/getAllUsers",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"users",
						"getAllUsers"
					]
				}
			},
			"response": []
		},
		{
			"name": "getAllIssue",
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"method": "GET",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"title\": \"stargate\",\r\n    \"description\": \"new payment method\",\r\n    \"owner\": 2,\r\n    \"assignTo\": 2,\r\n    \"type\": 1,\r\n    \"status\": 1\r\n   \r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/Issues/getAllIssues",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"Issues",
						"getAllIssues"
					]
				}
			},
			"response": []
		},
		{
			"name": "addIssue",
			"request": {
				"method": "PUT",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"title\": \"ews\",\r\n    \"description\": \"server down\",\r\n    \"owner\": 1,\r\n    \"assignTo\": 1,\r\n    \"type\": 1,\r\n    \"status\": 1\r\n   \r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/Issues/updateIssue/2",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"Issues",
						"updateIssue",
						"2"
					]
				}
			},
			"response": []
		},
		{
			"name": "getIssue",
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"method": "GET",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n    \"title\": \"priceline\",\r\n    \"description\": \"memoery issue\",\r\n    \"owner\": 1,\r\n    \"assignTo\": 1,\r\n    \"type\": 1,\r\n    \"status\": 1\r\n   \r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/Issues/assinged/100",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"Issues",
						"assinged",
						"100"
					]
				}
			},
			"response": []
		},
		{
			"name": "deleteIssue",
			"request": {
				"method": "DELETE",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "http://localhost:8080/Issues/deleteIssue/53",
					"protocol": "http",
					"host": [
						"localhost"
					],
					"port": "8080",
					"path": [
						"Issues",
						"deleteIssue",
						"53"
					]
				}
			},
			"response": []
		}
	]
}
