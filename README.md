#  E-Commerce

## Deployed Link 
![site](https://watch.screencastify.com/v/UH3oA49RvC7uruGgRbYa)

## Example Picture 
![site](/Screenshot%202022-11-04%20at%2010.50.52%20PM.png)

## Techonologies Used 
- Javascript - Used this package to start our inquierer prompt on our terminal, this allowed us to view the questions and select our answers.
- Insomnia - This technology allowed us to create databases with information logged into which we then modified correctly.

## Summary 
In this application we were able to create the database of a company, allowing us to view employees, their id, role in the company, and their managers, as well as their salaries.

## Code Snippet 
``` JavaScript 
router.delete('/:id', async (req, res) => {
  // delete one product by its `id` value
  try {
    const productData = await Product.destroy({
      where: {
        id: req.params.id
      }
    });
  
    if(!productData){
      res.status(404).json({message: 'No product found with this id'});
      return;
    }
   res.status(200).json({message: 'Destroyed ' + req.params.id});
  }catch (err) {
    res.status(500).json(err);
  }
});
``` 
## Author Links

[LinkedIn](https://www.linkedin.com/in/angel-matias-01120b251/)
[GitHub] (https://github.com/robogf)
