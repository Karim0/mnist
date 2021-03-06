# Text recognising
 
The project implemented a number recognition function (from 0 to 9).<br> Number is recognized in 3 ways:<br>

<ul>
  <li>Neural networks</li>
  <li>Random forest</li>
  <li>Decision Trees</li>
</ul>
The test results are as follows.

<table>
  <tr>
    <th>Way</th>
    <td>Studying time</td>
    <td>Score (test set)</td>
    <td>Params</td>
  </tr>
  
  <tr>
    <th>Neural networks</th>
    <td>1min</td>
    <td>93.99%</td>
    <td>input_nodes = 784 <br>hidden_nodes = 100 <br>output_nodes =10 <br>learning_rate =0.3</td>
  </tr>
  
  <tr>
    <th>Random forest</th>
    <td>3min 16s</td>
    <td>97.18%</td>
    <td>random_state=17<br>n_estimators=1000<br>n_jobs=-1</td>
  </tr>
  
  <tr>
    <th>Decision Trees</th>
    <td>51.4 s</td>
    <td>88.21%</td>
    <td>random_state=17<br>'max_depth': 16</td>
  </tr>
  
  <tr>
    <th>CNN model (tensorflow)</th>
    <td>6 min 13 s</td>
    <td>99.32%</td>
    <td>optimizer=Adam<br>
        loss=CategoricalCrossentropy</td>
  </tr>
</table>
<h2>CNN model structure</h2>
<img src="https://github.com/Karim0/mnist/blob/master/img/cnn_modal.png" alt="">
