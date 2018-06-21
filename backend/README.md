# Backend
Be the yin to the front-enders' yang. Give power to our awesome client-side experiences with equally awesome server-side ingenuity.

## Challenge Details
Wribbn does all things shopping. Not just online, but in the stores too. The challenge is to connect a user with the physical shops they love.

  1. Create a NodeJS server.
  2. Create a Mongo database with three collections (`users`, `products`, and `stores`) defined by Mongoose schemas.
      - `products` belong to stores
      - `users` can follow stores (you don't need to implement this behavior, just the structure)
      - `stores` and `users` have geo-locations
      - Any other meta information is fair game
  3. Populate your database with dummy data.
  4. Create two functions to aggregate the data in the following way:
      - Given a `user`, show a list of `product`s from the `store`s they follow.
      - Given a `user`, show a list of `store`s nearest to their specified location

## Guidelines
There's no need to build a front-end interface if you don't want to. Dumping results to the console is just fine.

## The Extra Mile
100% optional, but if you feel like going big!

  1. Update a `user`'s location on an interval to show nearby `store`s dynamically.
  2. Assuming `product`s can also be "liked" by `user`s, provide a list of the most "popular" `store`s:
      - Popularity is determined by the total number of likes on `product`s from each `store` AND by the number of `user`s who follow the `store`
  3. Pipe everything over Socket.IO to a browser console.
