# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romefrontend/js-parser/index.test.ts --update-snapshots` to update.

## `es2015 > uncategorised > 235`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "input.js"
		end: Object {
			column: 36
			index: 36
			line: 1
		}
		start: Object {
			column: 0
			index: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: "Loop variable declaration may not have an initializer"}
			}
			location: Object {
				filename: "input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 15
					index: 15
					line: 1
				}
				start: Object {
					column: 5
					index: 5
					line: 1
				}
			}
		}
	]
	body: Array [
		JSForInStatement {
			loc: Object {
				filename: "input.js"
				end: Object {
					column: 36
					index: 36
					line: 1
				}
				start: Object {
					column: 0
					index: 0
					line: 1
				}
			}
			right: JSReferenceIdentifier {
				name: "list"
				loc: Object {
					filename: "input.js"
					identifierName: "list"
					end: Object {
						column: 23
						index: 23
						line: 1
					}
					start: Object {
						column: 19
						index: 19
						line: 1
					}
				}
			}
			body: JSExpressionStatement {
				loc: Object {
					filename: "input.js"
					end: Object {
						column: 36
						index: 36
						line: 1
					}
					start: Object {
						column: 25
						index: 25
						line: 1
					}
				}
				expression: JSCallExpression {
					loc: Object {
						filename: "input.js"
						end: Object {
							column: 35
							index: 35
							line: 1
						}
						start: Object {
							column: 25
							index: 25
							line: 1
						}
					}
					callee: JSReferenceIdentifier {
						name: "process"
						loc: Object {
							filename: "input.js"
							identifierName: "process"
							end: Object {
								column: 32
								index: 32
								line: 1
							}
							start: Object {
								column: 25
								index: 25
								line: 1
							}
						}
					}
					arguments: Array [
						JSReferenceIdentifier {
							name: "x"
							loc: Object {
								filename: "input.js"
								identifierName: "x"
								end: Object {
									column: 34
									index: 34
									line: 1
								}
								start: Object {
									column: 33
									index: 33
									line: 1
								}
							}
						}
					]
				}
			}
			left: JSVariableDeclaration {
				kind: "let"
				loc: Object {
					filename: "input.js"
					end: Object {
						column: 15
						index: 15
						line: 1
					}
					start: Object {
						column: 5
						index: 5
						line: 1
					}
				}
				declarations: Array [
					JSVariableDeclarator {
						id: JSBindingIdentifier {
							name: "x"
							loc: Object {
								filename: "input.js"
								identifierName: "x"
								end: Object {
									column: 10
									index: 10
									line: 1
								}
								start: Object {
									column: 9
									index: 9
									line: 1
								}
							}
						}
						loc: Object {
							filename: "input.js"
							end: Object {
								column: 15
								index: 15
								line: 1
							}
							start: Object {
								column: 9
								index: 9
								line: 1
							}
						}
						init: JSNumericLiteral {
							value: 42
							format: undefined
							loc: Object {
								filename: "input.js"
								end: Object {
									column: 15
									index: 15
									line: 1
								}
								start: Object {
									column: 13
									index: 13
									line: 1
								}
							}
						}
					}
				]
			}
		}
	]
}
```

### `diagnostics`

```

 input.js:1:5 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Loop variable declaration may not have an initializer

    for (let x = 42 in list) process(x);
         ^^^^^^^^^^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```