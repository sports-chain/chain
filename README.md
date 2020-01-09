Public chain open source code

this is some of chain 


````go
func Sign(signer Signer, data []byte) ([]byte, error) {
	signature, err := s.Sign(signer.Scheme(), signer.PrivKey(), data, nil)
	if err != nil {
		return nil, err
	}

	return s.Serialize(signature)
}
````
