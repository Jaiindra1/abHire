  try {
      const response = await axios.post(
        'https://abhirebackend.onrender.com/clients/clients',
        form,
        {
          headers: {
            'accept': 'application/json',
            'Content-Type': 'application/json'
          }
        }
      );
      console.log('✅ Client saved:', response.data);
      alert('Client saved successfully!');
    } catch (error) {
      console.error('❌ Save failed:', error);
      alert('Failed to save client.');
    }
