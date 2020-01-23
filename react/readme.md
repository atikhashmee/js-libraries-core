#  This is react tutorial
here i will be creating components using class and function
- we are going to see function like this
```sh
so this is how it goes
```
and after that we be doing something like [facebook](www.facebook.com)


# React js Textarea
React js handle textarea with ```value```
so this will be similar to other to single line input, [see more](https://reactjs.org/docs/forms.html#the-textarea-tag)

## get the value from textarea 
```javascript
 bodyChangeHandler = (evt) => {
            const p = this.state.post;
            p.body = evt.target.value;
            this.setState({
                post :{...p}
                });
        }
```
```html
 <form onSubmit={this.formData}>
                                        <input type="text" className="form-control" name='name' onChange={this.titleChangeHandler} value={this.state.post.title} />
                                        <textarea  className="form-control" cols="30" onChange={this.bodyChangeHandler} value={this.state.post.body}   rows="10"></textarea>
                                        <button className="btn btn-success">Submit</button>
                                    </form>
```

# React Hook
==============================

So from React 16.8 , we can use `function` as components and let's you do the things you could do in a class `component`

*Important* thing to keep in mind while you using `CDN` that   `useState()` may throw an error 

so in order use it properly , we have to use `React.userState()` because its defined in the `React` object. 
[more](https://github.com/FormidableLabs/react-live/issues/114)

## example 
```javascript
 <div id="root"></div>
   <script type="text/babel">
        function Example(){
            const [count, setCount] =React.useState(0);
            return (
                    <div>
                        <p>You clicked {count} times</p>
                        <button onClick={() => setCount(count + 1)}>
                            Click me
                        </button>
                    </div>
            );
        }

       ReactDOM.render(<Example/>, document.getElementById('root'));
   </script>
```