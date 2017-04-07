# sinon-test
spy的作用在于，可以监视一个函数被调用的情况，例如： var spy = sinon.spy(object, "method")
stub用于在测试中控制一个方法的行为，以强制代码沿特定路径执行。
mock同spy的区别，mock出的object收到了数据或是调用并没有真正执行

https://medium.freecodecamp.com/simple-react-testing-d9e25ec87e2?gi=e7e552e9fa79
https://github.com/newyork-anthonyng/tutorials/blob/master/Simple_React_Testing/test/ajax_spec.js
https://github.com/airbnb/enzyme/issues/486


//////////////////////////////////////////////////////////////////////////
var Dummy = {
    doSomething: function(something) {
        return 'doing ...' + something;
    }
}

sinon.stub(Dummy, 'doSomething')
    .withArgs('sleep').returns('sleepy')
    .withArgs('eat').returns('eating');
    
console.log(Dummy.doSomething('sleep'));
console.log(Dummy.doSomething('eat'));

//////////////////////////////////////////////////////////////////////////
test on node
http://raathigesh.com/Mocking-HTTP-Requests-with-Axios-Mock-Adapter/

//////////////////////////////////////////////////////////////////////////
