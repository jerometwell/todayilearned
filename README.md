# todayilearned 👀💥🏥
Documenting myself banging my head on _the spiked wall of life_ , on repeat.

## Stupid problems that took Stupid me longer than they should have to solve

#### Ruby and and and and Chips
  Ruby has a different operator precedence for operators `&&` and `and`
  
#### Using the wrapped terraform option from the terraform github action prevents use of output variables
  https://blog.nillsf.com/index.php/2020/08/25/how-to-use-terraform-output-in-a-github-action/
  
#### S3 websites must be named with their external DNS
  It is not, as I previously thought, a convention. because the ALIAS record points to `s3-website-${region}.amazonaws.com.`, the host is used to resolve the bucket name.
  
#### jest resetMocks will reset manual "__mocks__" entirely
  clearMocks is what you want - but it was a surprise to find that the `__mocks__` features was getting completely obliterated on every test. It makes sense in retrospect: the mock is being set up in the `__mocks__` implementation. But I guess i assumed they would be treated differently.
