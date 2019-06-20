# Argparse2class for Jupyter execution.

Argparse transformation for Jupyter Notebook execution. (for quick testing in .ipynb)<br />
Copy & paste class-formatted arguments to replace argparse. <br/>

If you find some buggy outputs, please publish a issue or mail me : <u> sngjuk@gmail.com </u>
### latest update : Jun 20, 19
Jun 20, 19 : fix it add_option() available <br>

### bug to fix :
for now, not found.

### quick web transformation :
http://35.192.144.192:8000/arg2cls.html

### usage : 
```
python3 arg2cls.py [target.py] [target2.py(optional)] ...
```

### make argument parser into-
```
parser = argparse.ArgumentParser(description='PyTorch PennTreeBank RNN/LSTM Language Model')
parser.add_argument('--data', type=str, default='./data/penn',
                    help='location of the data corpus')
parser.add_argument('--model', type=str, default='LSTM',
                    help='type of recurrent net (RNN_TANH, RNN_RELU, LSTM, GRU)')
parser.add_argument('--emsize', type=int, default=200,
                    help='size of word embeddings')
parser.add_argument('--nhid', type=int, default=200,
                    help='number of hidden units per layer')
```
### class format
```
class args:
    data = './data/penn'
    model = 'LSTM'
    emsize = 200
    nhid = 200
```

### input (argparse lines) :

![alt text](http://pds27.egloos.com/pds/201709/01/00/c0134200_59a941fb9501e.png)


### ouput (args class) :

![alt text](http://thumbnail.egloos.net/600x0/http://pds25.egloos.com/pds/201709/01/00/c0134200_59a936974c78f.png)


### transformed usage : 
If there's no default value for argument, It will have warning value. (###manual_setting_required###)

![alt text](http://pds21.egloos.com/pds/201709/01/00/c0134200_59a937f65f737.png)
