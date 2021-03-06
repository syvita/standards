# Syv-03 - Unit Testing

- All pure functions require unit tests.
- All unit tests should follow the Arrange, Act, Assert (AAA) pattern.
- NodeJS projects should maintain tests in a folder `test` in the top-level of the project.
- `mocha`+`chai` or `jest` are good unit testing framework choices for NodeJS projects.
- NodeJS unit tests using `mocha` or `jest` should conform to the following format:
  1. The `describe` block is the message signature of the tested function.
  2. There is a **minimum** of one `it` block per return path for the function.
  3. Each `expect` assertion must include a debugging message logging the value tested to assist ease of debugging.

Here is an example of a conforming unit test...

```
/**
 * Dummy function to return 'foo' or 'bar'
 * @param baz A flag that if true, returns 'foo'. Else, returns 'bar'
 */
function foobar(baz: boolean): string {
  return baz ? "foo" : "bar";
}

describe("foobar(baz: boolean): string", () => {
  it("should return 'foo' if baz is true", () => {
    const baz = true; // Arrange

    const result = foobar(baz); // Act

    expect(result, `Result should be 'foo' when baz=${baz} is true`).to.equal(
      "foo"
    ); // Assert
  });

  it("should return 'bar' if baz is false", () => {
    const baz = false; // Arrange

    const result = foobar(baz); // Act

    expect(result, `Result should be 'bar' when baz=${baz} is false`).to.equal(
      "bar"
    ); // Assert
  });
});
```
