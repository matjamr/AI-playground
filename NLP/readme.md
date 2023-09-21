sth like RNN but for data
data should have at least 1 mln characters



BASIC NLP FLOW <br>
1.Read in Test Data <br>
2.Encode string to integers <br>
3.Create batches <br>
4.model embedding layer (cast single ints to dense vector) -> GRU -> Dense Layer
5.Train model