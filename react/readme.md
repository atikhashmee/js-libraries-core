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
```sh
 bodyChangeHandler = (evt) => {
            const p = this.state.post;
            p.body = evt.target.value;
            this.setState({
                post :{...p}
                });
        }
```
```
 <form onSubmit={this.formData}>
                                        <input type="text" className="form-control" name='name' onChange={this.titleChangeHandler} value={this.state.post.title} />
                                        <textarea  className="form-control" cols="30" onChange={this.bodyChangeHandler} value={this.state.post.body}   rows="10"></textarea>
                                        <button className="btn btn-success">Submit</button>
                                    </form>
```

