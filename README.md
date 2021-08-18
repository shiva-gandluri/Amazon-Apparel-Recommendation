# Amazon-Apparel-Recommendation 
   <h3>Problem:</h3>
    <p>
      Recommend products that are most similar to the current product to Amazon customers.
      Given a product, I’ve analysed it by its image, brand name, color etc and recommended products 
      which have most similar features to the current product.
    </p>
      
   <h3>Data:</h3>
    <p>
      The Amazon Apparel recommendation has around 0.18 million products with 7 features for each product. 
      The data contains both textual and image information as attributes such as product type(shirt, pant etc), product brand,
      product colour, product image etc.  
    </p>

   <h3>Approach:</h3>
    <p>
      <ul>
        <li>
          Performed Data Cleaning & Data Preprocessing by removing unnecessary and duplicates rows 
          and for text reviews removed HTML tags, punctuations, Stopwords and Stemmed the words using Porter Stemmer.
        </li>
        <li>
         For each product, found the most similar products using sklearns's cosine_similarity and pairwise_distances on
          <ul>
            <li>
              Textual Feature Vectors for product's 'Title', 'Brand', 'Type' attributes seperately.
            </li>
            <li>
              Weighted average textual Feature Vectors of product's 'Brand', 'Colour' attributes.
            </li>
            <li>
              Image Feature Vectors for product's Image attribute.
            </li>
          </ul>
        </li>
      </ul>
    </p>
      
   <b>Technologies Used:</b> Convolutional Neural Networks, Machine Learning, Python
   <br> <br>

