from cmd import Cmd
import requests

ip = input("Roku IP: ")

class Prompt(Cmd):
    prompt = 'roku> '
    intro = "Welcome to RokuCLI! Type ? to list commands"
 
    def do_up(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Up')
    def do_down(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Down')
    def do_left(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Left')
    def do_right(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Right')
    def do_select(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Select')
    def do_back(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Back')
    def do_replay(self, inp):
        requests.post('http://' + ip + ':8060/keypress/InstantReplay')
    def do_info(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Info')
    def do_reverse(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Rev')
    def do_play(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Play')
    def do_forward(self, inp):
        requests.post('http://' + ip + ':8060/keypress/Fwd')
    
 
if __name__ == '__main__':
    Prompt().cmdloop()