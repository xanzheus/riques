# homepage
My homepage

Keeping here snippets:

Bliking effect in unity:
			//blinking effect. hide if > .5 and show if <= .5
			if (tracking <= 5 && ((tracking*10)%10 > 5)){
				gameObject.transform.GetComponent<Text> ().text = "";
			}
