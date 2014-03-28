var assert = chai.assert;

suite('Tests', function(){

  test('Suma: ', function(){
    object = pl0.parse("x = 3 + 5 .")
    assert.equal(object.block.st.right.type, "+")
  });

  test('Multiplicacion: ', function(){
    object = pl0.parse("x = 4 * 1 .")
    assert.equal(object.block.st.right.type, "*") 
  });

  test('Division: ', function(){
    object = pl0.parse("x = 1 / 6 .")
    assert.equal(object.block.st.right.type, "/")
  });
test('Begin End: ', function(){
    object = pl0.parse("begin x = 3; z = b+3 end.")
    assert.equal(object.type, "program")
  });

  test('Error de Sintaxis: ', function(){
    assert.throws(function() { pl0.parse("x = 323"); }, /Expected "."/);
  });


});
