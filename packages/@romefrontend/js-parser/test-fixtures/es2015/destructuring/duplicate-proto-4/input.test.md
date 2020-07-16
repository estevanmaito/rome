# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romefrontend/js-parser/index.test.ts --update-snapshots` to update.

## `es2015 > destructuring > duplicate-proto-4`

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
			column: 0
			index: 54
			line: 2
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
				message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: "Redefinition of __proto__ property"}
			}
			location: Object {
				filename: "input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 26
					index: 26
					line: 1
				}
				start: Object {
					column: 17
					index: 17
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "input.js"
				end: Object {
					column: 53
					index: 53
					line: 1
				}
				start: Object {
					column: 0
					index: 0
					line: 1
				}
			}
			expression: JSArrowFunctionExpression {
				loc: Object {
					filename: "input.js"
					end: Object {
						column: 52
						index: 52
						line: 1
					}
					start: Object {
						column: 0
						index: 0
						line: 1
					}
				}
				body: JSBlockStatement {
					body: Array []
					directives: Array []
					loc: Object {
						filename: "input.js"
						end: Object {
							column: 52
							index: 52
							line: 1
						}
						start: Object {
							column: 50
							index: 50
							line: 1
						}
					}
				}
				head: JSFunctionHead {
					async: false
					hasHoistedVars: false
					rest: undefined
					returnType: undefined
					thisType: undefined
					loc: Object {
						filename: "input.js"
						end: Object {
							column: 49
							index: 49
							line: 1
						}
						start: Object {
							column: 0
							index: 0
							line: 1
						}
					}
					params: Array [
						JSBindingObjectPattern {
							rest: undefined
							loc: Object {
								filename: "input.js"
								end: Object {
									column: 45
									index: 45
									line: 1
								}
								start: Object {
									column: 1
									index: 1
									line: 1
								}
							}
							properties: Array [
								JSBindingObjectPatternProperty {
									key: JSStaticPropertyKey {
										value: JSIdentifier {
											name: "__proto__"
											loc: Object {
												filename: "input.js"
												identifierName: "__proto__"
												end: Object {
													column: 12
													index: 12
													line: 1
												}
												start: Object {
													column: 3
													index: 3
													line: 1
												}
											}
										}
										loc: Object {
											filename: "input.js"
											end: Object {
												column: 12
												index: 12
												line: 1
											}
											start: Object {
												column: 3
												index: 3
												line: 1
											}
										}
									}
									value: JSBindingIdentifier {
										name: "x"
										loc: Object {
											filename: "input.js"
											identifierName: "x"
											end: Object {
												column: 15
												index: 15
												line: 1
											}
											start: Object {
												column: 14
												index: 14
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
											column: 3
											index: 3
											line: 1
										}
									}
								}
								JSBindingObjectPatternProperty {
									key: JSStaticPropertyKey {
										value: JSIdentifier {
											name: "__proto__"
											loc: Object {
												filename: "input.js"
												identifierName: "__proto__"
												end: Object {
													column: 26
													index: 26
													line: 1
												}
												start: Object {
													column: 17
													index: 17
													line: 1
												}
											}
										}
										loc: Object {
											filename: "input.js"
											end: Object {
												column: 26
												index: 26
												line: 1
											}
											start: Object {
												column: 17
												index: 17
												line: 1
											}
										}
									}
									value: JSBindingIdentifier {
										name: "y"
										loc: Object {
											filename: "input.js"
											identifierName: "y"
											end: Object {
												column: 29
												index: 29
												line: 1
											}
											start: Object {
												column: 28
												index: 28
												line: 1
											}
										}
									}
									loc: Object {
										filename: "input.js"
										end: Object {
											column: 29
											index: 29
											line: 1
										}
										start: Object {
											column: 17
											index: 17
											line: 1
										}
									}
								}
								JSBindingObjectPatternProperty {
									key: JSStaticPropertyKey {
										value: JSIdentifier {
											name: "__proto__"
											loc: Object {
												filename: "input.js"
												identifierName: "__proto__"
												end: Object {
													column: 40
													index: 40
													line: 1
												}
												start: Object {
													column: 31
													index: 31
													line: 1
												}
											}
										}
										loc: Object {
											filename: "input.js"
											end: Object {
												column: 40
												index: 40
												line: 1
											}
											start: Object {
												column: 31
												index: 31
												line: 1
											}
										}
									}
									value: JSBindingIdentifier {
										name: "z"
										loc: Object {
											filename: "input.js"
											identifierName: "z"
											end: Object {
												column: 43
												index: 43
												line: 1
											}
											start: Object {
												column: 42
												index: 42
												line: 1
											}
										}
									}
									loc: Object {
										filename: "input.js"
										end: Object {
											column: 43
											index: 43
											line: 1
										}
										start: Object {
											column: 31
											index: 31
											line: 1
										}
									}
								}
							]
						}
					]
				}
			}
		}
	]
}
```

### `diagnostics`

```

 input.js:1:17 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Redefinition of __proto__ property

    ({ __proto__: x, __proto__: y, __proto__: z }) => {};
                     ^^^^^^^^^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```